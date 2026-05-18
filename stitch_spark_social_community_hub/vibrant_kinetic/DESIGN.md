---
name: Vibrant Kinetic
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#d2c1d4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#9b8c9e'
  outline-variant: '#4f4352'
  surface-tint: '#e9b3ff'
  primary: '#e9b3ff'
  on-primary: '#510074'
  primary-container: '#c863fb'
  on-primary-container: '#460066'
  inverse-primary: '#9026c3'
  secondary: '#aac7ff'
  on-secondary: '#003064'
  secondary-container: '#3e90ff'
  on-secondary-container: '#002957'
  tertiary: '#ffb2b7'
  on-tertiary: '#67001c'
  tertiary-container: '#ff506c'
  on-tertiary-container: '#5b0017'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f6d9ff'
  primary-fixed-dim: '#e9b3ff'
  on-primary-fixed: '#310048'
  on-primary-fixed-variant: '#7200a3'
  secondary-fixed: '#d6e3ff'
  secondary-fixed-dim: '#aac7ff'
  on-secondary-fixed: '#001b3e'
  on-secondary-fixed-variant: '#00468d'
  tertiary-fixed: '#ffdadb'
  tertiary-fixed-dim: '#ffb2b7'
  on-tertiary-fixed: '#40000e'
  on-tertiary-fixed-variant: '#91002b'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  h1:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  h2:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h3:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 40px
  xl: 64px
  container-max: 1280px
  gutter: 20px
---

## Brand & Style

This design system is engineered for a high-energy niche social ecosystem. It centers on the concept of "Digital Vitality," blending the depth of a sophisticated matte environment with the explosive energy of neon light. The brand personality is electric, forward-leaning, and deeply connected.

The visual style is a hybrid of **Glassmorphism** and **Bento-box minimalism**. By utilizing semi-transparent surfaces over dark backgrounds, the UI achieves a sense of physical depth. Glowing accents and multi-color gradients act as "energy paths" that guide the eye toward interactive elements, creating a rhythmic, high-contrast experience that feels both premium and underground.

## Colors

The color palette is anchored by a deep **Matte Black (#121212)** base, which provides the necessary contrast for the neon accents to "pop" without causing eye strain. 

- **Primary (Electric Purple):** Used for core branding and high-level navigation states.
- **Secondary (Neon Cyan):** Used for connectivity indicators, links, and secondary actions.
- **Tertiary (Hot Pink):** Reserved for alerts, notifications, and "live" status updates.
- **Surface Strategy:** Backgrounds use the base matte black, while cards and containers utilize a slightly lighter "off-black" (#1C1C1E) or semi-transparent glass layers to create separation. 
- **Glow Accents:** Critical interactive components should feature a subtle outer glow (drop shadow) matching their primary hex code to simulate light emission.

## Typography

This design system utilizes a high-contrast typographic hierarchy. **Inter** provides a clean, systematic foundation for both headings and body copy, ensuring legibility against dark backgrounds. 

For technical data, stats, and small utility labels, **Space Grotesk** is introduced to add a futuristic, geometric edge. Headlines should be styled with tight letter-spacing and heavy weights to command attention, while body text maintains generous line-heights to prevent "text-blooming" on OLED displays.

## Layout & Spacing

The layout philosophy follows a **Bento-box** structure, organizing information into modular, distinct cells of varying sizes. This approach uses a 12-column grid with fixed gutters to create a sense of organized density.

- **Grid Alignment:** All cards and containers must snap to the grid. 
- **Bento Logic:** Larger blocks (2x2 or 3x2) are used for featured content or media, while smaller blocks (1x1) house rapid-fire stats or quick-actions.
- **Inner Padding:** Consistent internal padding of 24px (md) is required for all containers to maintain visual breathability within the high-energy aesthetic.

## Elevation & Depth

Elevation is achieved through **Glassmorphism** and tonal layering rather than traditional shadows.

1.  **Level 0 (Floor):** The #121212 matte black background.
2.  **Level 1 (Cards):** Semi-transparent surfaces (rgba 255, 255, 255, 0.05) with a 20px backdrop-blur and a subtle 1px inner border (rgba 255, 255, 255, 0.1).
3.  **Level 2 (Active/Floating):** Higher transparency (rgba 255, 255, 255, 0.1) with a colored "glow" shadow matching the element's accent color (e.g., a purple glow for a primary button).

Avoid heavy, muddy black shadows. Instead, use "light-leaks"—soft, colored blurs that appear to sit behind glass panels—to indicate depth and hierarchy.

## Shapes

The shape language is consistently **Rounded**, striking a balance between organic fluidity and structural precision. 

- **Containers & Bento Boxes:** Use `rounded-xl` (1.5rem / 24px) to create a soft, modern container feel.
- **Interactive Elements:** Buttons and input fields use `rounded-lg` (1rem / 16px).
- **Avatars & Tags:** Use pill-shapes (full rounding) to contrast against the rectangular nature of the bento grid. 
- **Borders:** All glass elements should feature a thin, high-contrast stroke to define edges against the dark background.

## Components

- **Buttons:** Primary buttons use the "Hyper-flow" gradient with white text. Secondary buttons are "Ghost" style with a 1px neon cyan border and a matching glow on hover.
- **Bento Cards:** The foundational unit. Each card must have a 1px border and a subtle background blur. Headings within cards should be positioned in the top-left, with stats or actions in the bottom-right.
- **Glass Chips:** Small, semi-transparent badges used for tagging or status. They should utilize the primary/secondary colors at 20% opacity for the background and 100% for the text.
- **Inputs:** Darker than the card background (#000000) with a focus state that triggers a neon-cyan border glow.
- **Connection Lines:** Use thin, animated gradient strokes to connect related bento cards, visualizing the "Connected" aspect of the platform.
- **Glow-Toggles:** Custom switches that emit a hot-pink light when in the 'on' position, reflecting the high-energy theme.