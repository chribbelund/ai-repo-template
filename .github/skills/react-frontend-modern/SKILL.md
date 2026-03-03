---
name: react-frontend-modern
description: Build modern React frontends with TypeScript, component-driven architecture, accessible UI, reliable state/data fetching, and strong performance defaults. Use when creating or refactoring React pages, components, hooks, forms, and tests.
---

# React Frontend (Modern) Skill

Use this skill for React feature development and refactoring.

## When to Use This Skill

- Building new React features, pages, or shared components
- Refactoring components for clarity, reusability, and type safety
- Implementing forms, async flows, and API integration
- Improving performance and accessibility in existing UI

## Prerequisites

- Follow existing repo conventions (routing, state, styling, testing)
- Prefer TypeScript for all new React code
- Validate with existing lint/typecheck/test commands

## Workflow

1. Identify feature boundary and existing component/state patterns
2. Model types first (props, API models, UI state)
3. Build small composable components and custom hooks
4. Implement loading/empty/error/success states
5. Add accessibility semantics and keyboard support
6. Add tests for behavior and critical user paths

## Implementation Rules

- Prefer functional components and hooks.
- Keep components focused; extract logic to hooks when complexity grows.
- Avoid prop drilling when context/composition is more maintainable.
- Handle async state explicitly (pending/success/error).
- Co-locate tests with features unless repo patterns differ.
- Keep styling consistent with existing design system/tokens.

## Performance Defaults

- Memoize only where profiling shows benefit.
- Split large routes/components.
- Avoid unnecessary re-renders from unstable object/function props.
- Prefer list virtualization for very large collections.

## Accessibility Defaults

- Use semantic HTML before ARIA.
- Ensure full keyboard navigation and visible focus states.
- Provide accessible names/labels for controls.
- Ensure sufficient color contrast and non-color indicators.

## References

- [Component checklist](references/component-checklist.md)
- [A11y checklist](references/a11y-checklist.md)
