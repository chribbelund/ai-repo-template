---
applyTo: "**/*.ts,**/*.tsx,**/*.css,**/*.scss"
---
# React / Frontend Rules

- Use functional components and hooks.
- Prefer TypeScript for new UI logic.
- Keep components composable; extract complex logic into custom hooks.
- Handle loading, empty, error, and success states explicitly.
- Keep UI consistent with design system tokens and existing primitives.

## Accessibility

- Use semantic HTML first, ARIA only when needed.
- Ensure full keyboard interaction and visible focus states.
- Ensure labels, accessible names, and sufficient color contrast.

## Performance

- Avoid unnecessary re-renders from unstable props/dependencies.
- Split large routes/components when beneficial.
