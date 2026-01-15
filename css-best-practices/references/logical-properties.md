# Logical Properties for i18n

Use logical properties (start/end) instead of physical properties (left/right) to support multi-directional layouts.

## Examples

### Correct
```css
.message-bubble {
  margin-inline-start: 1rem;
  padding-inline-end: 2rem;
}
```

## Why it matters
Using logical properties makes it easier to support multi-directional layouts, such as right-to-left (RTL) languages. It also makes the code more readable and maintainable.