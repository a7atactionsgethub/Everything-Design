````md id="universal-avatar-code"
# 🎭 Hybrid Avatar System — Universal Implementation

## 📦 Installation

```bash
npm install @dicebear/core @dicebear/collection
```

---

# 📁 File Structure

```txt
src/
└── lib/
    └── avatar/
        └── getUserAvatar.ts
```

---

# ⚙️ `getUserAvatar.ts`

```ts
import { createAvatar } from "@dicebear/core";
import { lorelei } from "@dicebear/collection";

type AvatarUser = {
  uid: string;
  displayName?: string | null;
  photoURL?: string | null;
};

/**
 * Generate deterministic fallback avatar
 * using DiceBear.
 */
function generateFallbackAvatar(seed: string): string {
  return createAvatar(lorelei, {
    seed,

    size: 128,

    radius: 12,

    randomizeIds: true,

    backgroundColor: [
      "1e293b",
      "312e81",
      "0f172a",
      "1f2937",
    ],
  }).toDataUri();
}

/**
 * Hybrid Avatar Resolver
 *
 * Priority:
 * 1. External profile image
 * 2. DiceBear fallback avatar
 */
export function getUserAvatar(
  user: AvatarUser
): string {

  // Use existing profile image
  if (
    user.photoURL &&
    user.photoURL.trim() !== ""
  ) {
    return user.photoURL;
  }

  // Generate fallback avatar
  const seed =
    user.displayName?.trim() ||
    user.uid;

  return generateFallbackAvatar(seed);
}
```

---

# 🖼️ React Usage

```tsx
import { getUserAvatar } from "@/lib/avatar/getUserAvatar";

<img
  src={getUserAvatar(user)}
  alt="User Avatar"
  className="h-10 w-10 rounded-full object-cover"
/>
```

---

# 🔥 Firebase Google Auth Example

```ts
import {
  GoogleAuthProvider,
  signInWithPopup,
} from "firebase/auth";

import { auth } from "./firebase";

const provider = new GoogleAuthProvider();

async function loginWithGoogle() {
  try {

    const result = await signInWithPopup(
      auth,
      provider
    );

    const user = result.user;

    console.log(user.displayName);
    console.log(user.photoURL);

  } catch (error) {
    console.error(error);
  }
}
```

---

# 🧠 Logic Flow

```txt
IF Google profile image exists
    → use Google image

ELSE
    → generate DiceBear avatar
```

---

# ✅ Benefits

```txt
✓ No image uploads
✓ No storage required
✓ Deterministic fallback avatars
✓ Lightweight architecture
✓ Works with Firebase Auth
✓ Production-ready
✓ Easy to scale
```
````
