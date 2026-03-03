# Accessibility Checklist (React UI)

## Semantics

- Native elements used (`button`, `label`, `nav`, `main`, etc.)
- Heading hierarchy is logical
- Form controls have explicit labels

## Keyboard and Focus

- All interactive controls reachable by keyboard
- Focus order matches visual/logical order
- Focus styles are clearly visible
- Dialogs/menus manage focus correctly

## Visual Accessibility

- Text contrast meets WCAG AA baseline
- Touch targets are large enough for mobile interaction
- UI does not rely on color alone to communicate meaning

## Dynamic Content

- Validation errors are announced and clearly associated
- Loading and status updates are understandable to assistive tech
- Motion is reduced or optional where appropriate
