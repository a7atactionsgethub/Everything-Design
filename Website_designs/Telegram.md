# Design System Inspired by Telegram

## 1. Visual Theme & Atmosphere

Telegram's design system embodies a clean, minimal aesthetic prioritizing speed and accessibility. The visual personality is modern yet approachable, with a focus on clarity and directness. The interface uses a predominantly light background with purposeful pops of vibrant blue as the primary action color, creating strong visual hierarchy without visual clutter. The design encourages frictionless interaction through generous spacing, large touch targets, and intuitive information architecture. Telegram's visual language feels secure and trustworthy—professional without being corporate, friendly without being frivolous.

**Key Characteristics**
- Minimal, light-first design with selective color accents
- Large, legible typography with generous line height
- Blue-dominant accent system with supporting semantic colors
- Generous whitespace and breathing room between elements
- High contrast for accessibility and readability
- Rounded corners on interactive elements for approachability
- Zero-embellishment aesthetic with functional design focus

## 2. Color Palette & Roles

### Primary
- **Telegram Blue** (`#3390EC`): Primary CTA buttons, links, active states, and brand accent throughout the interface
- **Primary Variant** (`#3C87F7`): Alternative blue for secondary emphasis and interactive states

### Accent Colors
- **Purple** (`#8774E1`): Secondary brand accent for highlights and decorative elements
- **Vibrant Purple** (`#976FFF`): Enhanced purple for standout moments and gradient potential
- **Lime Green** (`#88D93A`): Accent for highlight and notification badges
- **Warm Orange** (`#FF845E`): Supporting accent for energy and call-to-action variety

### Interactive
- **Link Blue** (`#3390EC`): All link text and link-based interactions
- **Hover State Blue** (`#3C87F7`): Hover elevation of primary actions

### Neutral Scale
- **Pure Black** (`#000000`): Primary text, headings, and dominant UI elements
- **Dark Charcoal** (`#212121`): Secondary text and subtle UI elements
- **Dark Gray** (`#181818`): Tertiary text for muted content
- **Medium Gray** (`#707579`): Disabled states, placeholders, and helper text
- **Light Gray** (`#717579`): Border and divider lines
- **Off-White** (`#F4F4F5`): Subtle background tints and container fills

### Surface & Borders
- **Pure White** (`#FFFFFF`): Primary surface, modal backgrounds, and card surfaces
- **Border Gray** (`#DFE1E5`): Subtle borders, dividers, and section separators

### Semantic / Status
- **Success Green** (`#30B73B`): Primary success indicator and confirmation states
- **Success Light Green** (`#5CC85E`): Supporting success accent and active indicators
- **Warning Yellow** (`#FFAA00`): Primary warning state for caution messages
- **Warning Light Yellow** (`#FFCD3A`): Supporting warning accent for highlights
- **Error Red** (`#FF595A`): Primary error and destructive action indicator
- **Success Deep Green** (`#195530`): Supporting green for success container backgrounds

## 3. Typography Rules

### Font Family
**Primary Font:** Roboto (`font-family: 'Roboto', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`)

**Secondary Font:** Roboto (single family system)

Fallback stack: `Roboto, -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', sans-serif`

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| Display XL | Roboto | 48px | 500 | 52.8px | 0px | Page titles, hero sections |
| Display Large | Roboto | 40px | 500 | 44px | 0px | Major section headers |
| Heading 1 | Roboto | 36px | 500 | 39.6px | 0px | Page headings |
| Heading 2 | Roboto | 32px | 500 | 35.2px | 0px | Section headings |
| Heading 3 | Roboto | 28px | 500 | 30.8px | 0px | Subsection headings |
| Heading 4 | Roboto | 24px | 500 | 26.4px | 0px | Card titles |
| Body Large | Roboto | 18px | 400 | 25px | 0px | Lead text, intro copy |
| Body Regular | Roboto | 16px | 400 | 21px | 0px | Primary body text, list items |
| Body Small | Roboto | 14px | 400 | 19px | 0px | Secondary body, metadata |
| Button | Roboto | 16px | 400 | 24px | 0px | All button text |
| Link | Roboto | 16px | 400 | 21px | 0px | Hyperlink text |
| Caption | Roboto | 12px | 400 | 16px | 0px | Captions, helper text, timestamps |
| Code | Roboto | 13px | 400 | 18px | 0px | Monospace code blocks |

### Principles
- Clean, readable sans-serif provides modern, technical credibility
- Single font family simplifies implementation and ensures consistency
- Weight hierarchy uses 500 for headings, 400 for body to create clear distinction
- Generous line heights (1.3–1.5) ensure comfortable reading and visual breathing room
- Letter spacing remains at 0 for standard layouts, maintaining density without cramping
- All text rendering uses antialiasing for smooth appearance across devices

## 4. Component Stylings

### Buttons

#### Primary Button
- **Background:** `#3390EC`
- **Text Color:** `#FFFFFF`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `12px 24px`
- **Height:** `54px`
- **Border Radius:** `10px`
- **Border:** `0px none`
- **Box Shadow:** `0px 2px 8px rgba(0, 0, 0, 0.12)`
- **Hover:** Background `#2A7BD4`, Box Shadow `0px 4px 12px rgba(0, 0, 0, 0.16)`
- **Active:** Background `#2168BA`
- **Disabled:** Background `#D5E3F0`, Text Color `#999999`

#### Secondary Button (Link Style)
- **Background:** `transparent`
- **Text Color:** `#3390EC`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `0px`
- **Height:** `54px`
- **Border Radius:** `10px`
- **Border:** `0px none`
- **Box Shadow:** `none`
- **Hover:** Text Color `#3C87F7`
- **Active:** Text Color `#2A7BD4`
- **Disabled:** Text Color `#CCCCCC`

#### Ghost Button (Icon)
- **Background:** `transparent`
- **Text Color:** `#707579`
- **Font Size:** `24px`
- **Font Weight:** `400`
- **Padding:** `8px`
- **Height:** `auto`
- **Width:** `auto`
- **Border Radius:** `50%`
- **Border:** `0px none`
- **Box Shadow:** `none`
- **Line Height:** `24px`
- **Hover:** Background `rgba(51, 144, 236, 0.08)`
- **Active:** Background `rgba(51, 144, 236, 0.12)`

#### Text Button (Minimal)
- **Background:** `transparent`
- **Text Color:** `#000000`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `0px`
- **Height:** `40px`
- **Border Radius:** `0px`
- **Border:** `0px none`
- **Box Shadow:** `none`
- **Hover:** Text Color `#3390EC`
- **Active:** Text Color `#2A7BD4`

### Cards & Containers

#### Card Surface
- **Background:** `#FFFFFF`
- **Border:** `1px solid #DFE1E5`
- **Border Radius:** `10px`
- **Padding:** `20px`
- **Box Shadow:** `0px 1px 4px rgba(0, 0, 0, 0.08)`
- **Margin Bottom:** `16px`

#### Container
- **Background:** `#F4F4F5`
- **Border Radius:** `10px`
- **Padding:** `24px`
- **Margin Bottom:** `24px`

#### Modal Overlay
- **Background:** `rgba(0, 0, 0, 0.5)`
- **Box Shadow:** `0px 8px 32px rgba(0, 0, 0, 0.2)`

### Inputs & Forms

#### Text Input
- **Background:** `#FFFFFF`
- **Text Color:** `#000000`
- **Border:** `1px solid #DFE1E5`
- **Border Radius:** `10px`
- **Padding:** `12px 16px`
- **Font Size:** `16px`
- **Line Height:** `24px`
- **Focus:** Border `1px solid #3390EC`, Box Shadow `0px 0px 0px 3px rgba(51, 144, 236, 0.1)`
- **Placeholder Color:** `#707579`
- **Disabled:** Background `#F4F4F5`, Border Color `#DFE1E5`, Text Color `#999999`
- **Error:** Border `1px solid #FF595A`

#### Checkbox
- **Size:** `18px × 18px`
- **Border:** `2px solid #DFE1E5`
- **Border Radius:** `4px`
- **Background (Unchecked):** `#FFFFFF`
- **Background (Checked):** `#3390EC`
- **Check Color:** `#FFFFFF`
- **Focus:** Box Shadow `0px 0px 0px 3px rgba(51, 144, 236, 0.1)`

#### Radio Button
- **Size:** `18px × 18px`
- **Border:** `2px solid #DFE1E5`
- **Border Radius:** `50%`
- **Background (Unchecked):** `#FFFFFF`
- **Inner Circle (Checked):** `8px × 8px`, Background `#3390EC`
- **Focus:** Box Shadow `0px 0px 0px 3px rgba(51, 144, 236, 0.1)`

### Navigation

#### Navigation Item
- **Background:** `transparent`
- **Text Color:** `#707579`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `0px`
- **Height:** `48px`
- **Line Height:** `24px`
- **Hover:** Text Color `#3390EC`
- **Active:** Text Color `#3390EC`, Border Bottom `3px solid #3390EC`

#### Navigation Container
- **Background:** `#FFFFFF`
- **Border Bottom:** `1px solid #DFE1E5`
- **Padding:** `0px 20px`
- **Height:** `60px`

### Badges

#### Badge (Success)
- **Background:** `#30B73B`
- **Text Color:** `#FFFFFF`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 8px`
- **Border Radius:** `4px`

#### Badge (Warning)
- **Background:** `#FFAA00`
- **Text Color:** `#FFFFFF`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 8px`
- **Border Radius:** `4px`

#### Badge (Error)
- **Background:** `#FF595A`
- **Text Color:** `#FFFFFF`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 8px`
- **Border Radius:** `4px`

## 5. Layout Principles

### Spacing System
**Base Unit:** `8px`

**Spacing Scale:**
- `8px`: Tight spacing for related elements, icon-to-label padding
- `16px`: Standard margin between components, horizontal gutters
- `20px`: Vertical spacing, section padding
- `24px`: Major component spacing, container padding
- `40px`: Large padding for spacious layouts
- `48px`: Major vertical spacing between sections
- `172px`: Hero section bottom margin
- `180px`: Extra large spacing for section breaks

**Usage Context:**
- Micro-spacing (`8px`): Icon padding, small form inputs
- Standard spacing (`16px–24px`): Component margins, container padding, typical grid gaps
- Macro-spacing (`48px–180px`): Section breaks, hero sections, full-width layout rhythm

### Grid & Container
- **Max Width:** `1200px` (or full-width on mobile)
- **Column Strategy:** 12-column grid on desktop, 4-column on tablet, 2-column on mobile
- **Container Padding:** `20px` on mobile, `40px` on tablet, `60px` on desktop
- **Gutter Width:** `16px` between columns
- **Section Pattern:** Centered max-width container with uniform horizontal padding

### Whitespace Philosophy
Generous whitespace creates visual hierarchy and reduces cognitive load. Large margins between sections emphasize content importance. Tight micro-spacing within components maintains logical grouping. The design system prioritizes breathing room over information density, trusting users to scroll rather than cramming content vertically.

### Border Radius Scale
- `0px`: Sharp corners for text buttons and minimal components
- `4px`: Subtle rounding for badges and small form elements
- `10px`: Standard rounding for buttons, cards, and containers
- `50%`: Perfect circles for icon buttons and avatars

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat | `box-shadow: none` | Text-only buttons, navigation items, minimal UI |
| Raised | `box-shadow: 0px 1px 4px rgba(0, 0, 0, 0.08)` | Cards, input fields in focus, standard containers |
| Elevated | `box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.12)` | Primary buttons, hover states, interactive surfaces |
| Floating | `box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.16)` | Buttons in hover state, dropdowns, expanded menus |
| Modal | `box-shadow: 0px 8px 32px rgba(0, 0, 0, 0.2)` | Modal dialogs, overlays, highest elevation |

**Shadow Philosophy:**
Shadows are subtle and minimal, supporting functional depth rather than pure decoration. Low elevation levels (1–2px lift) provide feedback on interactive hover states. Higher elevations appear only on modals and floating elements to maintain visual clarity. All shadows use black at low opacity (`0.08–0.2`) to preserve the light aesthetic. This approach preserves the minimal design language while providing clear interactive affordance.

## 7. Do's and Don'ts

### Do
- Use `#3390EC` Telegram Blue for all primary CTAs and key interactive elements
- Maintain minimum `8px` padding around all interactive targets for comfortable touch zones
- Apply consistent `10px` border radius to all button and card components
- Use generous `24px` vertical spacing between major content sections
- Style links with `#3390EC` text color and underline on hover
- Employ `#FFFFFF` backgrounds with `#DFE1E5` borders for subtle contained surfaces
- Reserve semantic colors (`#30B73B`, `#FF595A`, `#FFAA00`) exclusively for status messaging
- Keep typography to Roboto with `400` weight for body and `500` for headings
- Provide minimum `44px` height for mobile touch targets
- Use box shadows at `0.08–0.12` opacity for subtle, accessible depth

### Don't
- Avoid background colors that reduce contrast below WCAG AA standards (4.5:1 for text)
- Never combine multiple primary blue accents in a single view; stick to one dominant `#3390EC` per section
- Don't use shadows heavier than `0px 8px 32px` for non-modal components; reserve high elevation for modals only
- Avoid mixing button styles within a single action group; maintain consistent primary/secondary distinction
- Don't reduce padding below `8px` for any interactive element
- Never override the base font family with other sans-serifs; Roboto is the system standard
- Avoid using custom border radius values outside the `0px / 4px / 10px / 50%` scale
- Don't apply opacity to semantic colors; use the provided palette variants instead
- Avoid text smaller than `12px` in any context, including captions
- Never apply both shadow and border to the same element; choose one depth cue

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | `0px–600px` | Single-column layout, full-width containers, `20px` horizontal padding, stacked navigation |
| Tablet | `600px–1024px` | 2–4 column grid, `40px` padding, condensed navigation, responsive typography |
| Desktop | `1024px+` | 12-column grid, `60px` padding, full navigation, max-width `1200px` container |

### Touch Targets
- **Minimum Size:** `44px × 44px` for all interactive elements on mobile
- **Button Height:** `54px` on mobile, `48px` on desktop
- **Icon Button Size:** `40px × 40px` minimum with `8px` internal padding
- **Touch Spacing:** Minimum `8px` gap between adjacent interactive elements
- **Link Underline:** Visible on hover, width `2px` for easy identification

### Collapsing Strategy
- **Typography:** Reduce body font from `16px` (desktop) to `14px` (tablet) to `13px` (mobile)
- **Spacing:** Decrease margins from `24px` (desktop) to `16px` (tablet) to `8px` (mobile)
- **Containers:** Stack full-width on mobile, enforce max-width on desktop
- **Navigation:** Horizontal desktop nav collapses to hamburger menu below `600px`
- **Grid Columns:** 12 columns (desktop) → 4 columns (tablet) → 2 columns (mobile)
- **Modal Width:** 90% on mobile, 80% on tablet, fixed `500px` on desktop
- **Image Scaling:** Maintain aspect ratio, scale down to fit container width with `max-width: 100%`

## 9. Agent Prompt Guide

### Quick Color Reference
- **Primary CTA:** Telegram Blue (`#3390EC`)
- **Primary CTA Hover:** Primary Variant (`#3C87F7`)
- **Background Surface:** Pure White (`#FFFFFF`)
- **Heading Text:** Pure Black (`#000000`)
- **Body Text:** Pure Black (`#000000`)
- **Secondary Text:** Medium Gray (`#707579`)
- **Disabled Text:** Medium Gray (`#707579`)
- **Border:** Border Gray (`#DFE1E5`)
- **Success Indicator:** Success Green (`#30B73B`)
- **Error Indicator:** Error Red (`#FF595A`)
- **Warning Indicator:** Warning Yellow (`#FFAA00`)
- **Subtle Container:** Off-White (`#F4F4F5`)

### Iteration Guide

1. **Start with blue:** All CTAs default to `#3390EC` unless explicitly overridden for secondary or tertiary actions.

2. **Apply 10px radius:** Every button, card, and contained input uses `border-radius: 10px` except text buttons (`0px`) and avatars (`50%`).

3. **Set base spacing:** Use `24px` margins between major sections, `16px` between components, `8px` for tightly grouped elements.

4. **Use Roboto 400/500:** Body text is Roboto `400` at `16px`; all headings are Roboto `500` (size varies by role).

5. **Target 44px height:** Every interactive element must be at least `44px` tall and `44px` wide on mobile for touch compliance.

6. **Add subtle shadows:** Apply `0px 2px 8px rgba(0, 0, 0, 0.12)` to buttons and `0px 1px 4px rgba(0, 0, 0, 0.08)` to cards; reserve heavier shadows for modals only.

7. **Prioritize contrast:** Ensure text-to-background contrast meets WCAG AA (4.5:1 minimum for body text, 3:1 for large text).

8. **Reserve semantic colors:** Use `#30B73B` only for success, `#FF595A` only for errors, `#FFAA00` only for warnings—never decoratively.

9. **Stack on mobile:** Enforce single-column layouts below `600px`; use full-width containers with `20px` padding.

10. **Validate accessibility:** All interactive elements must have focus states using `box-shadow: 0px 0px 0px 3px rgba(51, 144, 236, 0.1)` and keyboard navigation support.