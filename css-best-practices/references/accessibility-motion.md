# Accessibility & Motion

Respect user preferences for reduced motion using the `prefers-reduced-motion` media query.

## Examples

### Correct
```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation: none !important;
  }
}
```

## Why it matters
Respecting user preferences for reduced motion is important for accessibility. It allows users to control animations and transitions that can cause motion sickness or seizures.