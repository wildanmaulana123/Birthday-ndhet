---
name: Nocturne Gala
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#ccc3d4'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#958e9e'
  outline-variant: '#4a4452'
  surface-tint: '#d3bbff'
  primary: '#d3bbff'
  on-primary: '#3f0689'
  primary-container: '#4c1d95'
  on-primary-container: '#b994ff'
  inverse-primary: '#6f46b9'
  secondary: '#ddb8ff'
  on-secondary: '#490081'
  secondary-container: '#62259b'
  on-secondary-container: '#d1a1ff'
  tertiary: '#d1c79d'
  on-tertiary: '#363113'
  tertiary-container: '#b4ab84'
  on-tertiary-container: '#453f20'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ebdcff'
  primary-fixed-dim: '#d3bbff'
  on-primary-fixed: '#260059'
  on-primary-fixed-variant: '#572ba0'
  secondary-fixed: '#f0dbff'
  secondary-fixed-dim: '#ddb8ff'
  on-secondary-fixed: '#2c0051'
  on-secondary-fixed-variant: '#62259b'
  tertiary-fixed: '#ede3b8'
  tertiary-fixed-dim: '#d1c79d'
  on-tertiary-fixed: '#201c02'
  on-tertiary-fixed-variant: '#4d4727'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 24px
  gutter: 16px
  section-gap: 64px
---

## Brand & Style
The brand personality is celebratory, sophisticated, and intimate. It aims to evoke the feeling of an exclusive midnight garden party or a high-end gala under a starlit sky. The aesthetic balance leans heavily into luxury and "sweetness," achieved through the interplay of deep regal tones and soft, ethereal glows.

The design system utilizes **Glassmorphism** as its primary stylistic driver. This creates a sense of depth and lightness against the dark, high-contrast background. Surfaces appear as translucent frosted glass, allowing the background's star shader to peak through, while soft shadows and gold accents provide the tactile premium feel required for a luxury birthday experience.

## Colors
The palette is anchored in a celestial spectrum:
- **Primary (Deep Purple):** Used for structural depth and brand presence. It acts as the core "ink" of the design.
- **Secondary (Soft Lavender):** Used for interactive elements, highlights, and soft glows. It provides the "sweetness" to the palette.
- **Accent (Cream/Gold):** Reserved strictly for high-level text highlights, celebratory badges, and ornate borders.
- **Background (Very Dark Indigo):** A deep base (`#020617` or `#0f172a`) that provides the necessary contrast for glass effects and star shader visibility.

Backgrounds should use a subtle radial gradient of the Primary color over the Neutral base to create a sense of atmospheric lighting.

## Typography
This design system employs a classic "Serif for Headlines, Sans for Utility" pairing to establish a premium editorial feel. 

**Playfair Display** provides the elegance and character needed for celebratory messaging and names. It should be used with tighter letter spacing in larger sizes. **Inter** handles all functional information, ensuring readability against complex glass backgrounds. Use wide tracking for labels to enhance the "luxury" feel of the UI.

## Layout & Spacing
The layout follows a **fluid grid** model with generous white space (or "dark space") to maintain a sense of luxury and calm. 

- **Desktop:** 12-column grid with 24px gutters and 80px side margins.
- **Mobile:** Single column with 24px side margins.
- **Rhythm:** Vertical spacing should be ample. Components are grouped in "islands" (glass cards) with a 64px gap between major sections to prevent the UI from feeling cluttered. Content should be center-aligned for hero sections to maximize the "invitation" feel.

## Elevation & Depth
Depth is conveyed through **Glassmorphism** and soft, tinted shadows rather than traditional gray-scale shadows.

1.  **Base Layer:** The star shader/background.
2.  **Mid Layer (Cards):** Background-blur (12px to 20px) with a semi-transparent Lavender fill (opacity 10-15%). A 1px border with a linear gradient (top-left: White @ 20%, bottom-right: Lavender @ 5%) adds a "sharp" glass edge.
3.  **High Layer (Modals/Popups):** Increased blur (40px) and a subtle outer glow using the Primary color (`#4c1d95`) at low opacity to simulate a neon aura.

Floating animations (subtle 5px Y-axis translation) should be applied to cards to enhance the feeling of weightlessness.

## Shapes
The shape language is ultra-soft and organic. 
- **Cards & Containers:** Use `rounded-2xl` (1.5rem / 24px) to emphasize the "sweet" and approachable nature of the birthday theme.
- **Buttons:** Use fully rounded (pill-shaped) ends for a modern, friendly touch.
- **Inputs:** Match the card roundedness (0.75rem to 1rem) to maintain consistency.

## Components
- **Buttons:** Primary buttons use a gradient of Primary-to-Secondary. Hover states should trigger a subtle glow effect. Text is white or high-contrast Cream.
- **Glass Cards:** The signature component. Must include a `backdrop-filter: blur()` and a thin, light border.
- **Chips/Badges:** Small, pill-shaped elements with a Cream background and Deep Purple text for high-priority labels like "VIP" or "Featured."
- **Inputs:** Transparent backgrounds with a Lavender bottom-border only, or a fully enclosed glass style. Placeholder text should be a muted Lavender.
- **Transitions:** Use `cubic-bezier(0.4, 0, 0.2, 1)` for all fade-ins. Elements should slide up slightly (20px) as they fade in to create a "revealing" effect.
- **Special Component (Countdown):** Use large Playfair Display numbers for a birthday countdown, styled with a Gold-to-Cream linear gradient fill.