# <img src="docs/assets/icon.png" width="40" height="40" /> LapLab: UI Design Specification

> [!IMPORTANT]
> **LapLab** is a high-performance precision environment. All design decisions must prioritize **data legibility** and **sub-millisecond accuracy**.

---

## 1. Visual Theme & Atmosphere
The LapLab design system, **"Velocity Glass,"** is engineered for high-precision data analysis. It creates a focused, immersive environment through a deep dark foundation layered with translucent, blurred glass surfaces.

![Design Preview](docs/assets/preview.png)

### Core Aesthetics
- **Foundation**: Deep charcoal backgrounds to minimize eye strain.
- **Elevation**: Depth is established through `backdrop-blur` (Glassmorphism).
- **Emphasis**: High-contrast accents (Emerald and Racing Red) guide the user.

---

## 2. Color Palette

| Role | Color | HEX | Usage |
| :--- | :--- | :--- | :--- |
| **Dark Base** | ![](https://img.shields.io/badge/-#111113-111113) | `#111113` | Main application background. |
| **Dark Surface** | ![](https://img.shields.io/badge/-#1C1C21-1C1C21) | `#1C1C21` | Secondary backgrounds for cards. |
| **Border** | ![](https://img.shields.io/badge/-#33333A-33333A) | `#33333A` | Defining geometry. |
| **Emerald Apex** | ![](https://img.shields.io/badge/-#10B981-10B981) | `#10B981` | Success and optimal performance. |
| **Racing Red** | ![](https://img.shields.io/badge/-#EF4444-EF4444) | `#EF4444` | Errors and critical limits. |
| **Challenger Blue** | ![](https://img.shields.io/badge/-#3B82F6-3B82F6) | `#3B82F6` | Primary rival telemetry. |

---

## 3. Typography

**Primary Font Family**: Inter (Geometric Sans-Serif)

```mermaid
graph LR
    H1["Display H1 (32px)"] --- H2["Heading H2 (24px)"]
    H2 --- Body["Primary Body (14px)"]
    Body --- Detail["Detail Body (12px)"]
    Detail --- Micro["Micro Data (9px)"]
```

| Role | Size | Weight | Line Height | Case |
| :--- | :--- | :--- | :--- | :--- |
| **Display H1** | 32px | 700 | 40px | Uppercase |
| **Heading H2** | 24px | 700 | 32px | Uppercase |
| **Card Title** | 18px | 700 | 24px | Uppercase |
| **Primary Body** | 14px | 400 | 20px | Normal |

---

## 4. Component Design Language

### Buttons
- **Primary**: High-contrast Off-White surface with Dark text.
- **Secondary**: Dark semi-transparent surface with light text.
- **Corner Radius**: `12px` (Standardized).

> [!TIP]
> Use **Glow Effects** (`box-shadow`) sparingly to highlight the active "Apex" state or critical failures.

---

## 5. Layout & Spacing

**Base Unit**: `4px`

```mermaid
pie title Spacing Distribution
    "Internal Padding (8-16px)" : 40
    "Component Gaps (24px)" : 30
    "Section Gaps (48px+)" : 30
```

### Responsive Strategy
- **Mobile**: Single column stack; 44px touch targets.
- **Desktop**: Full 12-column telemetry grid; 98% container width.
