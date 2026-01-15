# Container-First Responsiveness

Use Container Queries to style components based on their parent's size.

## Examples

### Correct
```css
.card-wrapper {
  container-type: inline-size;
}

@container (min-width: 400px) {
  .card { 
    display: flex; 
    gap: 1rem; 
  }
}
```

## Why it matters
Using container queries allows for more dynamic and responsive styling within components, decoupling from the viewport and enabling better component reusability.