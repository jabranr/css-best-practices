# Performance & Compositor Animations

Only animate properties that the browser can handle on the compositor thread (transform and opacity).

## Examples

### Correct
```css
.dropdown {
  transition: transform 0.3s, opacity 0.3s;
  transform: scaleY(1);
  transform-origin: top;
}
```

## Why it matters
Animating properties like `transform` and `opacity` allows the browser to use the compositor thread for animations, which is faster and more efficient than animating properties that require layout or paint.