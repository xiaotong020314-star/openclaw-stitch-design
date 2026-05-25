---
name: OpenClaw
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#404752'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#707883'
  outline-variant: '#bfc7d4'
  surface-tint: '#0061a4'
  primary: '#0061a4'
  on-primary: '#ffffff'
  primary-container: '#2f9bf7'
  on-primary-container: '#003156'
  inverse-primary: '#9ecaff'
  secondary: '#00687a'
  on-secondary: '#ffffff'
  secondary-container: '#57dffe'
  on-secondary-container: '#006172'
  tertiary: '#494bd6'
  on-tertiary: '#ffffff'
  tertiary-container: '#878bff'
  on-tertiary-container: '#1000a6'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d1e4ff'
  primary-fixed-dim: '#9ecaff'
  on-primary-fixed: '#001d36'
  on-primary-fixed-variant: '#00497d'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#e1e0ff'
  tertiary-fixed-dim: '#c0c1ff'
  on-tertiary-fixed: '#07006c'
  on-tertiary-fixed-variant: '#2f2ebe'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  container-margin: 20px
  gutter: 12px
---

## Brand & Style

The design system is centered on the persona of a **Seamless Life Assistant**. It targets busy professionals and proactive individuals who require an AI-native butler that feels intelligent, responsive, and deeply trustworthy. The emotional goal is "effortless mastery"—the user should feel that their life is being managed with precision and calm.

The visual style is **Corporate / Modern** with a strong emphasis on **Glassmorphism**. It leverages high-quality typography and strategic translucent layers to evoke a sense of high-tech sophistication. The interface feels "alive" through subtle pulsing states and depth, reflecting its proactive AI nature without being overwhelming.

## Colors

The palette is anchored by **Brand Blue (#2f9bf7)**, representing stability and intelligence. Supporting accents of **Cyan** and **Indigo** create a vibrant, tech-forward spectrum used for interactive states and AI-driven highlights.

- **Primary:** Actionable elements, primary branding, and active AI focus.
- **Secondary/Tertiary:** Used for data visualization and distinguishing between different categories of assistant tasks.
- **Backgrounds:** Utilize `Slate-50` for a crisp light mode and `Slate-900` for a deep, focused dark mode.
- **Semantics:** Emerald is strictly for success or active "listening" states; Rose is reserved for critical alerts or emergency interventions.

## Typography

This design system utilizes **Hanken Grotesk** for its clean, sharp, and contemporary feel, ensuring the UI feels modern and professional. For technical and functional data, **Geist** provides a mono-influenced precision that reinforces the "AI-native" developer-grade reliability.

Hierarchy is maintained through significant weight contrast and generous line heights to ensure readability during quick glances. Display sizes use tighter letter spacing for a more "locked-in" editorial look.

## Layout & Spacing

The system employs a **mobile-first fluid grid**. The spacing rhythm is based on a 4px baseline, ensuring all elements align to a predictable vertical and horizontal cadence.

- **Mobile:** 4-column layout with 20px outside margins.
- **Tablet:** 8-column layout with 32px outside margins.
- **Desktop:** 12-column fixed-width container (max-width 1280px).

Margins between related components (like cards in a stack) should use `md` (16px), while distinct sections of the application use `xl` (32px) to provide breathable whitespace and reduce cognitive load.

## Elevation & Depth

Hierarchy is established through **Ambient Shadows** and **Glassmorphism**. 

- **Level 1 (Base):** Slate-50 background.
- **Level 2 (Cards):** White background with `shadow-soft` (0px 4px 20px rgba(0,0,0,0.05)).
- **Level 3 (AI Toasts/Overlays):** 80% opacity backgrounds with a 16px backdrop-blur, creating a sense of being "on top" of the system.
- **Floating Actions:** Use a stronger indigo-tinted shadow to indicate they are primary touchpoints.

Shadows should never be pure black; they must be tinted with the background hue (e.g., a Slate-900 tint in dark mode) to maintain a natural, cohesive look.

## Shapes

The design system uses **Rounded** geometry to feel approachable and modern. 

- **Cards and Containers:** 1rem (16px) radius for standard containers.
- **Buttons and Chips:** Fully rounded (Pill-shaped) to encourage interaction and signify touch-friendliness.
- **AI Toasts:** Use `rounded-xl` (1.5rem) to differentiate them from standard structural cards, giving them a softer, bubble-like appearance.

## Components

### Proactive AI Toasts
Floating notification cards that appear at the top or center of the screen. They must feature a glassmorphic background, a primary icon in the brand blue, and clear dual-action buttons (e.g., "Approve" / "Reschedule").

### Buttons
- **Primary:** Full Brand Blue fill with white text, pill-shaped.
- **Secondary:** Transparent with a 1px border of Brand Blue.
- **Ghost:** No border, Indigo text, used for less frequent actions.

### Status Indicators
The assistant’s "presence" is indicated by a pulsing avatar. Use a CSS animation or Lottie file to create a soft, breathing glow effect (Primary to Cyan) when the AI is processing or listening.

### Cards
Clean containers with 16px padding. Icons should be sourced from **Remix Icon** for a consistent, lightweight weight. Headlines within cards use `headline-md` and body text uses `body-md`.

### Input Fields
Soft Slate-100 fills with no border in their resting state. On focus, the border transitions to 1px Brand Blue with a subtle outer glow.