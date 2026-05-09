# Design System Inspired by LapLab

## 1. Visual Theme & Atmosphere

LapLab's design system embodies precision and performance analytics through a modern, minimalist aesthetic. The visual language combines a deep dark palette with crisp neutral accents, creating a professional racing analysis environment that prioritizes data clarity and user focus. The interface employs subtle elevation and refined spacing to guide attention without visual noise, reflecting the meticulous nature of sim racing performance tracking. Frosted glass effects and soft shadows establish a contemporary, sophisticated atmosphere that balances technical complexity with accessible usability.

**Key Characteristics**
- Dark-first color scheme emphasizing focus and data legibility
- Minimal elevation through soft shadows and subtle borders
- Frosted glass effects on cards and navigation elements
- Generous whitespace supporting cognitive clarity
- High contrast between content and background for accessibility
- Modern, geometric design with refined corner treatments
- Inter typography system for clean, technical readability

## 2. Color Palette & Roles

### Primary
- **Dark Base** (`#09090B`): Primary background and text for maximum contrast; used throughout UI structure (25 instances)
- **Dark Variant** (`#18181B`): Secondary dark surface for layered depth and component backgrounds
- **Dark Tertiary** (`#1C1C21`): Subtle variation for hover states and nested elements

### Accent Colors
- **Dark Charcoal** (`#33333A`): Deep accent for interactive element states
- **Near Black** (`#111113`): Extreme dark for maximum emphasis on critical elements
- **Red Accent** (`#7F1D1D`): Deep maroon for secondary actions or warning highlights

### Interactive
- **Primary CTA** (`#09090B`): Primary button background with high contrast
- **Primary Text on CTA** (`#FFFFFF`): Text on dark CTAs for maximum readability
- **Secondary CTA** (`#FFFFFF`): Secondary button background maintaining hierarchy
- **Secondary CTA Text** (`#09090B`): Dark text on light secondary buttons

### Neutral Scale
- **Light Border** (`#E4E4E7`): Primary border color used throughout UI; most versatile neutral (67 instances)
- **Off White** (`#FAFAFA`): Nearly white surface for subtle backgrounds
- **Pure White** (`#FFFFFF`): Brightest neutral for maximum contrast elements
- **Light Gray** (`#F4F4F5`): Soft surface for secondary containers
- **Light Neutral** (`#F3F4F6`): Tertiary light surface
- **Medium Gray** (`#71717A`): Medium neutral for secondary text
- **Muted Gray** (`#A1A1AA`): Muted neutral for tertiary text

### Surface & Borders
- **Card Surface** (`#FFFFFF` at 70% opacity): Frosted glass effect on card components
- **Card Border** (`#E4E4E7` at 50% opacity): Subtle card boundaries
- **Navigation Surface** (`#FAFAFA` at 50% opacity): Translucent navigation bar background

### Semantic / Status
- **Error State** (`#EF4444`): Critical errors, destructive actions, and validation failures

## 3. Typography Rules

### Font Family
**Primary:** Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif

**Secondary:** Inter (same stack; Inter serves dual purpose for all text roles)

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|----------------|----|
| Display / H1 | Inter | 32px | 700 | 40px | -0.02em | Page titles and major headers |
| Heading H2 | Inter | 28px | 700 | 36px | -0.01em | Section headers and key callouts |
| Heading H3 | Inter | 24px | 700 | 32px | 0em | Card titles and subsection headers |
| Large Body | Inter | 16px | 400 | 24px | 0em | Primary body text and nav items |
| Body | Inter | 14px | 400 | 20px | 0em | Standard paragraph and form text |
| Body Medium | Inter | 14px | 500 | 20px | 0em | Emphasized body text and buttons |
| Caption | Inter | 12px | 400 | 16px | 0em | Helper text and captions |
| Link | Inter | 16px | 400 | 24px | 0em | Navigation links and inline links |
| Link Small | Inter | 14px | 400 | 20px | 0em | Small text links and secondary navigation |

### Principles
- Inter provides optimal screen legibility with consistent letterforms across all weights
- Hierarchy relies on size and weight variation; color maintains accessibility
- 1.4–1.5x multiplier between hierarchy steps ensures visual distinction
- Line height set to 1.4–1.5x font size for comfortable reading on dark backgrounds
- Font weight limited to 400 (Regular) and 500–700 (Bold/Heavy) for clarity; no thin or light weights used
- All text meeting WCAG AA contrast requirements on respective backgrounds

## 4. Component Stylings

### Buttons

#### Primary Button
- **Background:** `#09090B`
- **Text Color:** `#FFFFFF`
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Padding:** `8px 16px`
- **Border Radius:** `6px`
- **Border:** `0px solid transparent`
- **Height:** `36px`
- **Box Shadow:** `0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)`
- **Hover State:** Background `#1C1C21`, shadow enhanced to `0px 2px 4px rgba(0, 0, 0, 0.15)`
- **Active State:** Background `#111113`
- **Disabled State:** Opacity `0.5`, cursor `not-allowed`

#### Secondary Button
- **Background:** `#FFFFFF`
- **Text Color:** `#09090B`
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Padding:** `8px 16px`
- **Border Radius:** `6px`
- **Border:** `1px solid #E4E4E7`
- **Height:** `36px`
- **Box Shadow:** `0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)`
- **Hover State:** Background `#F4F4F5`, border `1px solid #D4D4D7`
- **Active State:** Background `#E4E4E7`
- **Disabled State:** Opacity `0.5`, cursor `not-allowed`

#### Ghost Button
- **Background:** `transparent`
- **Text Color:** `#09090B`
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Padding:** `8px 16px`
- **Border Radius:** `6px`
- **Border:** `1px solid #E4E4E7`
- **Height:** `36px`
- **Box Shadow:** `none`
- **Hover State:** Background `#FAFAFA`, border `1px solid #D4D4D7`
- **Active State:** Background `#F4F4F5`
- **Disabled State:** Opacity `0.5`, cursor `not-allowed`

#### Icon Button
- **Background:** `transparent`
- **Text Color:** `#09090B`
- **Font Size:** `16px`
- **Padding:** `0px`
- **Border Radius:** `6px`
- **Border:** `0px solid transparent`
- **Width:** `36px`
- **Height:** `36px`
- **Box Shadow:** `none`
- **Hover State:** Background `#F4F4F5`
- **Active State:** Background `#E4E4E7`

### Cards & Containers

#### Standard Card
- **Background:** `rgba(255, 255, 255, 0.7)` (frosted glass effect)
- **Text Color:** `#09090B`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `24px`
- **Border Radius:** `12px`
- **Border:** `1px solid rgba(228, 228, 231, 0.5)`
- **Box Shadow:** `0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)`
- **Hover State:** Border `1px solid rgba(228, 228, 231, 0.8)`, shadow enhanced
- **Line Height:** `24px`

#### Dark Card
- **Background:** `#09090B`
- **Text Color:** `#FFFFFF`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `24px`
- **Border Radius:** `12px`
- **Border:** `1px solid #18181B`
- **Box Shadow:** `0px 1px 3px rgba(0, 0, 0, 0.3)`
- **Line Height:** `24px`

#### Elevated Container
- **Background:** `#FFFFFF`
- **Text Color:** `#09090B`
- **Padding:** `32px`
- **Border Radius:** `12px`
- **Border:** `1px solid #E4E4E7`
- **Box Shadow:** `0px 4px 12px rgba(0, 0, 0, 0.08)`

### Inputs & Forms

#### Text Input
- **Background:** `transparent`
- **Text Color:** `#09090B`
- **Font Size:** `14px`
- **Font Weight:** `400`
- **Padding:** `4px 12px`
- **Border Radius:** `6px`
- **Border:** `1px solid #E4E4E7`
- **Height:** `36px`
- **Box Shadow:** `0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)`
- **Focus State:** Border `1px solid #09090B`, box-shadow `0px 0px 0px 3px rgba(9, 9, 11, 0.1)`
- **Placeholder Color:** `#A1A1AA`
- **Line Height:** `20px`

#### Input Label
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Color:** `#09090B`
- **Margin Bottom:** `8px`
- **Line Height:** `20px`

#### Input Error State
- **Border:** `1px solid #EF4444`
- **Background:** `rgba(239, 68, 68, 0.05)`

#### Input Success State
- **Border:** `1px solid #10B981`
- **Background:** `rgba(16, 185, 129, 0.05)`

#### Form Group
- **Margin Bottom:** `16px`
- **Gap between label and input:** `8px`

### Navigation

#### Navbar Container
- **Background:** `rgba(250, 250, 250, 0.5)` (frosted translucent)
- **Text Color:** `#09090B`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `4px`
- **Border Radius:** `999px` (pill-shaped)
- **Border:** `1px solid #E4E4E7`
- **Height:** Auto (minimum `48px`)
- **Box Shadow:** `none`
- **Line Height:** `24px`

#### Nav Link
- **Background:** `transparent`
- **Text Color:** `#09090B`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `12px 16px`
- **Border Radius:** `6px`
- **Hover State:** Background `#F4F4F5`
- **Active State:** Background `#E4E4E7`, font-weight `500`
- **Line Height:** `24px`

#### Nav Link Secondary
- **Background:** `transparent`
- **Text Color:** `#09090B`
- **Font Size:** `14px`
- **Font Weight:** `400`
- **Padding:** `8px 12px`
- **Border Radius:** `4px`
- **Hover State:** Background `#FAFAFA`
- **Active State:** Background `#E4E4E7`, font-weight `500`
- **Line Height:** `20px`

### Badges

#### Default Badge
- **Background:** `#F4F4F5`
- **Text Color:** `#09090B`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 12px`
- **Border Radius:** `6px`
- **Border:** `1px solid #E4E4E7`

#### Primary Badge
- **Background:** `#09090B`
- **Text Color:** `#FFFFFF`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 12px`
- **Border Radius:** `6px`
- **Border:** `0px solid transparent`

#### Status Badge (Error)
- **Background:** `rgba(239, 68, 68, 0.1)`
- **Text Color:** `#EF4444`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 12px`
- **Border Radius:** `6px`
- **Border:** `1px solid #EF4444`

### Dividers
- **Color:** `#E4E4E7`
- **Height:** `1px`
- **Margin:** `16px 0px`

## 5. Layout Principles

### Spacing System

**Base Unit:** `4px`

**Scale:**
- `4px` — Tight spacing, small component gaps
- `8px` — Compact spacing, button/input internals, small list gaps
- `12px` — Small section spacing, form field gaps
- `16px` — Standard spacing, margin between components, padding in cards
- `24px` — Medium section spacing, primary card/container padding
- `32px` — Large spacing, section padding
- `48px` — XL spacing, major section breaks
- `64px` — Page-level spacing, top-level container margins

**Usage Context:**
- Buttons: `8px 16px` (vertical × horizontal)
- Cards: `24px` or `32px` padding
- Form groups: `16px` margin-bottom
- Section spacing: `48px` between major sections
- Component gaps: `12px` in grids, flex layouts

### Grid & Container

**Max Width:** `1440px` (full viewport or container limit for large displays)

**Column Strategy:** 12-column grid at desktop; 6-column at tablet; 4-column at mobile

**Section Patterns:**
- Hero/login sections: Centered, max-width `448px`–`512px`
- Content cards: Grid of 2–3 columns at desktop, 1–2 at tablet, 1 at mobile
- Dashboard panels: Flexible grid with `1fr` columns, minimum `320px` per card
- Form layouts: Single column at all breakpoints for clarity

### Whitespace Philosophy

The design system prioritizes generous whitespace to reduce cognitive load and emphasize data hierarchy. Spacing is intentional: large gaps between major sections create visual breathing room, while tight spacing within component groups maintains logical relationships. Dark backgrounds naturally increase perceived whitespace; this is leveraged to separate content without additional visible borders.

### Border Radius Scale

- `0px` — Hard edges for specific components (lines, separators)
- `4px` — Minimal rounding on small UI elements
- `6px` — Buttons, small cards, input fields, badges
- `12px` — Standard cards, larger containers, modals
- `999px` — Pill-shaped navigation, fully rounded elements (navigation pills, circular badges)

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat | No shadow, border only | Inputs, flat dividers, minimal components |
| Level 1 | `0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)` | Standard cards, buttons, form elements |
| Level 2 | `0px 2px 4px rgba(0, 0, 0, 0.15), 0px 2px 6px rgba(0, 0, 0, 0.1)` | Hovered cards, raised buttons, dropdowns |
| Level 3 | `0px 4px 12px rgba(0, 0, 0, 0.2), 0px 4px 8px rgba(0, 0, 0, 0.1)` | Modals, popovers, elevated containers |
| Level 4 | `0px 8px 24px rgba(0, 0, 0, 0.25), 0px 8px 12px rgba(0, 0, 0, 0.15)` | Floating action buttons, toast notifications |

**Shadow Philosophy:** Shadows in LapLab are purposefully subtle and restrained. The system employs soft, multi-layered shadows (multiple box-shadow values) to create perceived depth without visual heaviness. Shadows increase on hover to indicate interactivity. Dark backgrounds reduce shadow visibility; instead, subtle borders and color shifts convey elevation. This restraint maintains the clean, professional aesthetic while preserving hierarchy.

## 7. Do's and Don'ts

### Do

- **Use dark backgrounds** (`#09090B`, `#18181B`) for primary surfaces and maximum focus
- **Pair dark text** (`#09090B`) **with light backgrounds** (`#FFFFFF`, `#FAFAFA`) for optimal contrast
- **Apply frosted glass effects** (`rgba(255, 255, 255, 0.7)` with `1px solid rgba(228, 228, 231, 0.5)`) to cards for visual sophistication
- **Implement multi-layered shadows** for depth; use Level 1 as default, increase on interactive states
- **Use `#E4E4E7`** for all borders; it is the universal neutral border color (67 instances in codebase)
- **Maintain consistent `6px` border-radius** on buttons and form inputs
- **Use `12px` border-radius** on cards and larger containers
- **Space form elements** with `8px` between label and input, `16px` between form groups
- **Employ Inter typography** across all text roles; ensure legibility on dark backgrounds
- **Reserve `#EF4444`** strictly for error states, validation failures, and destructive actions
- **Apply generous padding** (`24px`–`32px`) in cards to support whitespace philosophy

### Don't

- **Do not mix border colors.** Always use `#E4E4E7` or its transparent variants; never introduce arbitrary grays
- **Do not use thin font weights** (300, 200, 100). Stick to `400 (Regular)` and `500–700 (Bold/Heavy)` only
- **Do not apply shadows to input fields.** Inputs use borders only; shadows indicate elevation, which inputs do not have
- **Do not exceed `1440px` container width** on desktop displays
- **Do not use red** (`#EF4444`) **for informational or success states.** Reserve it exclusively for errors and destructive actions
- **Do not nest more than 3 levels of component elevation.** Keep visual hierarchy simple and scannable
- **Do not apply rounded corners** beyond `12px` except for fully circular or pill-shaped elements (`999px`)
- **Do not use opacity** below `0.7` for card backgrounds; maintain legibility and visual integrity
- **Do not override the `16px`–`24px` spacing system** with arbitrary values; stick to the scale
- **Do not use secondary colors** (`#18181B`, `#1C1C21`) **as primary text.** These are background variants only
- **Do not apply line-height** below `1.4x` font size; this compromises readability on dark backgrounds
- **Do not hide the border on secondary buttons.** The `1px solid #E4E4E7` border is essential for visual distinction

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|------------|
| Mobile | `0px–639px` | 4-column grid, full-width containers, stacked navigation, `16px` padding |
| Tablet | `640px–1023px` | 6-column grid, 2-column card layouts, condensed nav, `24px` padding |
| Desktop | `1024px–1439px` | 12-column grid, 3-column cards, full nav, `32px` padding |
| Large | `1440px+` | Max-width container `1440px`, centered, consistent `32px` padding |

### Touch Targets

- **Minimum height:** `44px` for interactive elements (buttons, links, nav items)
- **Minimum width:** `44px` for clickable areas
- **Recommended padding:** `8px–12px` around touch targets to prevent accidental activation
- **Spacing between buttons:** Minimum `8px` to avoid overlap
- **Icon buttons:** `36px × 36px` for desktop, `44px × 44px` for mobile

### Collapsing Strategy

- **Mobile (< 640px):** Hide secondary navigation; collapse to hamburger menu. Stack card grids to single column. Reduce padding to `16px`. Consolidate form fields to full width. Hide decorative elements.
- **Tablet (640px–1023px):** Show primary navigation; secondary nav collapses conditionally. Display 2-column grid for cards. Maintain `24px` padding. Form fields at full width or 2-column grid. Show most content except minor secondaries.
- **Desktop (≥ 1024px):** Full navigation visible. 3-column card grid. Standard `32px` padding. Multi-column form layouts. All decorative elements visible. Max-width container centered.

## 9. Agent Prompt Guide

### Quick Color Reference

- **Primary CTA:** Dark Base (`#09090B`)
- **Primary CTA Text:** Pure White (`#FFFFFF`)
- **Secondary CTA:** Pure White (`#FFFFFF`)
- **Secondary CTA Text:** Dark Base (`#09090B`)
- **Background (Primary):** Dark Base (`#09090B`)
- **Background (Secondary):** Dark Variant (`#18181B`)
- **Card Surface:** Pure White at 70% opacity (`rgba(255, 255, 255, 0.7)`)
- **Card Border:** Light Border at 50% opacity (`rgba(228, 228, 231, 0.5)`)
- **Heading Text:** Dark Base (`#09090B`)
- **Body Text:** Dark Base (`#09090B`) or Muted Gray (`#A1A1AA`) for secondary
- **Input Border:** Light Border (`#E4E4E7`)
- **Error State:** Error Red (`#EF4444`)
- **Border (Universal):** Light Border (`#E4E4E7`)

### Iteration Guide

1. **Color Foundation:** All backgrounds use dark palette (`#09090B`, `#18181B`); all borders are `#E4E4E7`; never introduce custom colors outside the defined palette.
2. **Typography:** Use Inter font exclusively. Body text is `14px` weight `400`. Headlines are `24px` weight `700`. Buttons are `14px` weight `500`. Never deviate from extracted sizes.
3. **Spacing:** Apply `4px` base unit scaling: buttons `8px 16px`, cards `24px`–`32px` padding, form spacing `8px` (label-to-input), `16px` (group-to-group).
4. **Buttons:** Primary is dark (`#09090B` bg, `#FFFFFF` text). Secondary is light (`#FFFFFF` bg, `#09090B` text, `#E4E4E7` border). Ghost is transparent with border. All are `36px` height with `6px` radius.
5. **Cards:** Always use `12px` border-radius, `1px solid rgba(228, 228, 231, 0.5)` border, and Level 1 shadow (`0px 1px 3px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.1)`).
6. **Forms:** Inputs are `36px` height, `6px` radius, `1px solid #E4E4E7` border, `4px 12px` padding. Labels are `14px` weight `500`. No background color on inputs (transparent). Focus state adds `0px 0px 0px 3px rgba(9, 9, 11, 0.1)`.
7. **Shadows:** Use Level 1 shadow by default; increase to Level 2 on hover. Never apply shadows to flat elements (inputs, dividers). Dark backgrounds reduce shadow visibility—rely on borders instead.
8. **Whitespace:** Maintain generous padding and margins. Use the `4px` scale rigidly. Never compress spacing below recommended values; this reduces legibility and usability.
9. **Accessibility:** Ensure all text meets WCAG AA contrast. Dark text on light backgrounds, light text on dark backgrounds. Test interactive states (hover, focus, active) for clarity.
10. **Responsive:** Apply breakpoints at `640px` (mobile), `1024px` (desktop), `1440px` (large). Adjust grid columns, padding, and layout accordingly. Always maintain `44px` minimum touch target.