# Reading Notes 14a - CSS Animation

## Animation
- `transform` propert can be used to alter size, position, and elements.
- `transform` has two different settings, 2D and 3D.
- Example:
```CSS
  .selector {
    transform: rotate(20deg);
    transform: scale(.75);
    transform: scale(.5, 1.15);
    transform: translate(-10px, 25%);
    transform: skew(5deg, -20deg);
    transform: perspective(200px) rotateX(45deg);
  }
```

- `transition` alters the appearance or behavior of an element.
- 4 total `transition` properties: `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`.
- 8 simple CSS Transitions:
  1. Fade-in
  2. Change Color
  3. Grow & Shrink
  4. Rotate Element
  5. Square to Circle
  6. 3D Shadow
  7. Swing
  8. Inset Border

[Back to HOME](../README.md)