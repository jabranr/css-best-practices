# Layout Stability

Prevent Cumulative Layout Shift (CLS) by reserving space for media elements and dynamic containers before they load. Use of `aspect-ratio` can be impactful to prevent CLS.

## Description

Browsers need to know the dimensions of an element to calculate the layout. If an image or video loads without a defined size, the content below it will "jump" once the asset arrives.

## Examples

### Incorrect
```css
.hero-image {
  width: 100%;
  height: auto;
}
```

### Correct
```css
.hero-image {
  width: 100%;
  aspect-ratio: 16 / 9;
  object-fit: cover;
}
```

## Why it matters
Unexpected layout shifts are a primary metric in Google's Core Web Vitals.