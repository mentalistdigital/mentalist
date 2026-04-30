# Project Guidelines

These guidelines define styling and generation preferences for this project.

## General
- Prefer responsive layout patterns (flexbox/grid) over absolute positioning.
- Keep files focused; split reusable helpers/components into separate files.
- Refactor touched code when it improves clarity without changing behavior.
- Use semantic HTML and accessible labels/roles by default.

## Typography
- Display font: `Space Grotesk`
- Body font: `Manrope`
- Include these variables at root level:

```css
:root {
  --font-display: 'Space Grotesk', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-body: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

## Button Styling
### Glass Button
Use `.glass-button` for primary glassmorphism CTA actions.

Required characteristics:
- Light translucent background with blur
- Fully rounded pill radius (`9999px`)
- Soft layered shadow + inset highlights
- Subtle scale-up hover and scale-down active transitions

### Dark Glass Button
Use `.glass-button-dark` for glass buttons shown on light backgrounds.

Required characteristics:
- Dark translucent fill with blur
- Darker border and shadow model
- Same motion behavior as `.glass-button`

## Motion
- Keep transitions around `0.3s` with smooth cubic-bezier easing.
- Keep hover effects subtle and performance-safe.

## Design Intent
- Aim for premium, clean, modern UI.
- Prefer high legibility and restrained effects over decorative complexity.
