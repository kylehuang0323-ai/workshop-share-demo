# DESIGN.md

## Visual Style

- Register: brand
- Tone: professional, trustworthy, modern
- Density: medium (presentation-friendly scanning)
- Strategy: restrained + committed accent

## Color System (OKLCH)

- `--color-bg: oklch(1 0 0)`
- `--color-surface: oklch(0.972 0.004 112)`
- `--color-ink: oklch(0.23 0.02 112)`
- `--color-muted: oklch(0.46 0.012 112)`
- `--color-primary: oklch(0.56 0.12 112)`
- `--color-accent: oklch(0.36 0.08 148)`
- `--color-border: oklch(0.9 0.01 112)`

## Typography

- Family: `"Segoe UI", "Inter", -apple-system, BlinkMacSystemFont, sans-serif`
- Heading: 700 weight, balanced wrapping
- Body: 400-500 weight, max line length 72ch
- Scale: fluid `clamp()` for h1/h2 and section spacing

## Layout

- Max content width: `min(1120px, 92vw)`
- Hero + section rhythm with variable vertical spacing
- Grid for 2D content blocks (`auto-fit minmax`)
- Sticky top nav for meeting/demo navigation

## Components

- Header/Nav: compact sticky bar with clear anchors
- Hero: clear value statement + primary CTA
- Demo tiles: title, value statement, status, action link
- Timeline strip: workshop collaboration steps
- CTA panel: single clear next action

## Motion

- Subtle rise/fade on cards and section reveal
- Easing: cubic-bezier(0.22, 1, 0.36, 1)
- Reduced motion: transitions disabled under `prefers-reduced-motion`
