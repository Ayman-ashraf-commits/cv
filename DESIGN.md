---
name: Engineering Precision & Artifacts
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#ffb4ab'
  on-secondary: '#670507'
  secondary-container: '#871f1b'
  on-secondary-container: '#ff9a8e'
  tertiary: '#ffffff'
  on-tertiary: '#313030'
  tertiary-container: '#e5e2e1'
  on-tertiary-container: '#656464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#ffdad6'
  secondary-fixed-dim: '#ffb4ab'
  on-secondary-fixed: '#410002'
  on-secondary-fixed-variant: '#871f1b'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Bricolage Grotesque
    fontSize: 84px
    fontWeight: '800'
    lineHeight: 90px
  display-xl-mobile:
    fontFamily: Bricolage Grotesque
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 52px
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  code-sm:
    fontFamily: Geist Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  annotation:
    fontFamily: Caveat
    fontSize: 20px
    fontWeight: '400'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1100px
  section-gap: 8rem
  gutter: 1.5rem
  card-padding: 2rem
---

## Brand & Style

The design system is built for a "Product Builder" persona—someone who bridges the gap between high-level engineering and meticulous craft. The aesthetic is a fusion of **Technical Minimalism** and **Humanist Artifacts**. It balances the cold, precise world of code with the warm, spontaneous nature of product ideation.

- **Minimalism:** Use of expansive dark space, rigid grids, and high-contrast typography to emphasize clarity and focus.
- **Humanist Accents:** Integration of hand-drawn annotations and "doodles" to represent the sketching and ideation phase of building.
- **Atmospheric Depth:** A dark-mode first approach using subtle radial gradients and dashed strokes to mimic blueprints and digital canvases.

## Colors

The palette is intentionally restrained to allow content and work samples to command attention.

- **Foundation:** The background is a deep `#0a0a0a`, providing a void-like canvas that eliminates visual noise.
- **Accents:** The "Rust" red (`#b8433a`) is reserved exclusively for human elements—doodles, underlines, and hand-written annotations. This color should never be used for systematic UI like buttons or links.
- **Surfaces:** Cards and containers use `#1a1a1a` with low-opacity dashed borders to maintain a "work-in-progress" or "blueprint" feel.
- **Text:** Primary information is pure White (`#ffffff`), while metadata and descriptions use muted grays (`#a3a3a3`) to establish a clear information hierarchy.

## Typography

Typography is used as a structural element. 

- **Display & Headings:** Use **Bricolage Grotesque** (substituting for a custom bold serif) in uppercase for top-level headers. Its quirky yet bold geometry fits the "builder" narrative.
- **Body:** **Inter** provides high readability for long-form project descriptions and professional history.
- **Technical Detail:** **Geist Mono** is used for all tech stacks, metrics, and mono-spaced labels, emphasizing the "Full-Stack" nature of the work.
- **Annotations:** **Caveat** is used for "scribbled" notes, providing a direct contrast to the rigid Geist Mono.

## Layout & Spacing

This design system utilizes a **Fixed Grid** approach for the main content area to ensure a premium, editorial feel, while components within the grid remain fluid.

- **Structure:** A 12-column grid centered within a 1100px container.
- **Vertical Rhythm:** Sections are separated by large gaps (`8rem`) to provide breathing room and signal distinct transitions between About, Experience, and Projects.
- **Mobile Adaptivity:** On mobile, the 12-column grid collapses to 1 column, and section spacing reduces to `4rem`. Large display type scales down significantly to prevent awkward word breaks.
- **Navigation:** A top-fixed navigation bar with a heavy backdrop blur (`20px`) and a thin bottom border (`#ffffff10`).

## Elevation & Depth

This design system avoids traditional box shadows in favor of **Tonal Layering** and **Interactive Light**.

- **Surfaces:** Depth is created by the contrast between the `#0a0a0a` background and the `#1a1a1a` card surfaces.
- **Borders:** Instead of solid lines, use `1px dashed #ffffff20` for card containers. This reinforces the "schematic" aesthetic.
- **Interactive Light:** A global radial gradient follows the user's mouse cursor. The gradient is subtle (`radial-gradient(600px circle at var(--x) var(--y), rgba(255,255,255,0.06), transparent 40%)`).
- **Hover States:** Upon hovering over cards, the border should transition to a solid line or a brighter white, and the background should subtly lift to `#222222`.

## Shapes

The shape language is sharp and professional.

- **Primary Radius:** Use a soft `0.25rem` (4px) radius for cards and buttons. This keeps the design looking modern without appearing "bubbly."
- **Badges:** Tech stack badges and metric tags use a higher roundedness (`rounded-xl` or 12px) to differentiate them as small, pill-shaped UI elements.
- **Hand-drawn Elements:** Doodles (arrows, circles, underlines) should have an organic, variable stroke width to look authentic.

## Components

- **Navigation:** Simple text-based links using Geist Mono. Include a "Photo/Illustration Toggle" switch that uses a pill-shaped slider.
- **Experience Cards:** Features a dashed border, a Geist Mono date range at the top-right, and a bulleted list of achievements in Inter.
- **Project Cards:** Large, high-contrast headline. Tech stacks are displayed as a row of Geist Mono labels with a subtle background fill. Include a "Solo Shipped" badge in the top corner where applicable.
- **Metrics Tags:** Small containers with a subtle border and Geist Mono text (e.g., "+40% Conversion").
- **Doodle Overlay:** Position the `Caveat` text and `#b8433a` SVG doodles absolutely relative to the section headers or specific metrics to act as visual "marginalia."
- **Input Fields:** Bottom-border only (`1px solid #ffffff20`) with labels in Geist Mono. Focus state transitions the border to the accent red.