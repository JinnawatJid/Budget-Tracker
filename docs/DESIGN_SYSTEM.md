---
name: Friendly Finance
colors:
  surface: '#fff8f3'
  surface-dim: '#e2d8cd'
  surface-bright: '#fff8f3'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fdf2e6'
  surface-container: '#f7ece0'
  surface-container-high: '#f1e7db'
  surface-container-highest: '#ebe1d5'
  on-surface: '#1f1b14'
  on-surface-variant: '#4f4536'
  inverse-surface: '#353028'
  inverse-on-surface: '#faefe3'
  outline: '#817564'
  outline-variant: '#d3c5b0'
  surface-tint: '#7c5800'
  primary: '#7c5800'
  on-primary: '#ffffff'
  primary-container: '#e9b44c'
  on-primary-container: '#644600'
  inverse-primary: '#f4be55'
  secondary: '#2d6482'
  on-secondary: '#ffffff'
  secondary-container: '#a7dbfe'
  on-secondary-container: '#29617f'
  tertiary: '#804f6e'
  on-tertiary: '#ffffff'
  tertiary-container: '#e7abcf'
  on-tertiary-container: '#6b3d5b'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdea7'
  primary-fixed-dim: '#f4be55'
  on-primary-fixed: '#271900'
  on-primary-fixed-variant: '#5e4200'
  secondary-fixed: '#c6e7ff'
  secondary-fixed-dim: '#99cdf0'
  on-secondary-fixed: '#001e2d'
  on-secondary-fixed-variant: '#0a4c69'
  tertiary-fixed: '#ffd8ed'
  tertiary-fixed-dim: '#f2b5d9'
  on-tertiary-fixed: '#330c29'
  on-tertiary-fixed-variant: '#653856'
  background: '#fff8f3'
  on-background: '#1f1b14'
  surface-variant: '#ebe1d5'
typography:
  display-lg:
    fontFamily: Quicksand
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Quicksand
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Quicksand
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
  headline-md:
    fontFamily: Quicksand
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  label-md:
    fontFamily: Quicksand
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Quicksand
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 40px
  container-max: 1200px
---

## Brand & Style
This design system embraces a **Modern Flat Illustration** aesthetic, specifically drawing from the "Corporate Memphis" movement but infused with a tactile, zine-inspired warmth. The personality is approachable, non-intimidating, and optimistic—crucial for a budget tracking app that seeks to reduce financial anxiety.

The visual style is characterized by heavy, deliberate outlines and a "sticker-book" layout. It rejects the clinical cleanliness of traditional fintech in favor of a playful, hand-crafted feel. Key elements include grainy textures, solid offset shadows that suggest physical layers without using blurs, and a vibrant but soft pastel palette. The goal is to make every financial interaction feel like an inviting, creative exercise rather than a chore.

## Colors
The palette is rooted in a warm, pale peach background that provides a softer reading experience than pure white. The accent colors—Mustard, Sky, Pink, and Sage—are desaturated pastels that feel vibrant but grounded.

- **Primary (Mustard):** Used for key actions and progress highlights.
- **Secondary/Tertiary (Sky/Pink):** Used for categorizing different spending types.
- **Quaternary (Sage):** Used for positive financial trends or "on budget" statuses.
- **Neutral Stroke:** A deep charcoal used for all outlines and text to maintain high contrast and a "drawn" aesthetic.

Color is never used in gradients. Every surface is a solid fill, occasionally topped with a subtle noise/grain texture to add depth.

## Typography
**Quicksand** is the sole typeface for this design system, chosen for its rounded terminals and friendly, accessible geometry.

To maintain the "illustrative" feel, headlines are set in Bold (700) with slightly tighter letter-spacing. Body text utilizes Medium (500) weights to ensure legibility while maintaining the soft character of the brand. Numbers in financial readouts should always use the Bold weight to stand out against the thick outlines of their containers.

## Layout & Spacing
The design system utilizes a **fixed-width grid** approach for desktop to maintain the "sticker-sheet" composition, while fluidly scaling for mobile.

- **Grid:** 12-column layout on desktop, 4-column on mobile.
- **Rhythm:** An 8px base unit governs all padding and margins.
- **Structure:** Content is housed in cards that often "stack" visually. Spacing between cards should be generous (24px or 32px) to allow the thick outlines room to breathe without feeling cluttered.
- **Reflow:** On mobile, side-by-side cards stack vertically, and horizontal scrolling is used exclusively for category chips or "quick-add" budget items.

## Elevation & Depth
This design system rejects Gaussian blurs and soft shadows. Instead, depth is communicated through **Sticker Shadows** and **Tonal Layering**:

1.  **Level 0 (Background):** The pale peach base layer.
2.  **Level 1 (Cards/Elements):** Elements have a 2px dark charcoal outline.
3.  **Level 2 (Interaction/Focus):** When an element is active or hovered, it displays a hard, offset shadow (4px down, 4px right) in a darker version of the element's fill color or the neutral stroke color.
4.  **Grain:** A subtle, low-opacity noise overlay is applied to all Level 1 surfaces to give them a paper-like quality.

## Shapes
The shape language is dominated by high-radius curves. Most interactive elements use a **Pill-shaped (3)** configuration.

- **Buttons & Chips:** Always fully rounded (pill-shaped).
- **Cards:** Use a large 24px or 32px corner radius (`rounded-xl` equivalents).
- **Inputs:** Use a pill-shaped container for search and a 16px radius for larger text areas.
- **Outlines:** All shapes must have a consistent 2px stroke (3px for large display elements) to maintain the illustrative integrity.

## Components

### Buttons
Buttons are pill-shaped with a 2px dark outline. The primary button uses the Mustard fill with a "sticker" shadow that disappears (moves 0,0) when pressed, simulating a physical push.

### Cards
Cards use pastel fills (Sky, Pink, Sage) with a 2px dark border. They do not use shadows by default unless they are interactive. Information inside cards should be padded by at least 24px.

### Inputs
Input fields are white or pale peach with a 2px dark outline. The label sits above the field in a bold `label-md` style. When focused, the outline thickness increases to 3px or changes to the Primary Mustard color.

### Chips & Tags
Used for budget categories (e.g., "Food", "Rent"). These are small pill shapes with a 2px border. They can use the quaternary (Sage) color to indicate "under budget" or tertiary (Pink) for "over budget."

### Icons
Icons must be chunky and illustrative. Avoid thin lines. Use solid fills with the same 2px outline as the UI components. Icons should look like small "stickers" or emojis rather than abstract symbols.

### Progress Bars
Budget trackers use thick, rounded progress bars with a 2px outline. The background of the bar is a darker tint of the peach, and the fill is one of the accent pastels.
