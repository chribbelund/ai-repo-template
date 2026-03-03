# React Component Checklist

## Architecture

- Single responsibility: component has one clear purpose
- Public props are typed and minimal
- Complex logic extracted into custom hooks

## UX States

- Loading state present
- Empty state present
- Error state present with recovery path
- Success/confirmation state present when relevant

## Data and State

- Side effects are isolated and cleaned up
- Network state is handled deterministically
- Local vs global state choice is intentional

## Quality

- Behavior tests cover main interactions
- Edge cases are tested (invalid inputs, async failures)
- No obvious unnecessary renders from unstable dependencies
