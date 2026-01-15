# Maintainability & Cascade

Manage CSS specificity using Cascade Layers (@layer) and avoid high-specificity selectors.

## Examples

### Correct
```css
@layer base, components, utilities;

@layer base {
  a { 
    color: blue; 
  }
}

@layer components {
  .nav-link { 
    color: var(--brand-primary); 
  }
}

@layer utilities {
  .text-red { 
    color: red; 
  }
}
```

## Why it matters
Using Cascade Layers helps to manage the order of styles and avoid specificity issues. It also makes the code more maintainable and easier to understand.