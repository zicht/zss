# Padding

ZSS contains utility classes for setting values for the `padding` property.

## Source files

- [utilities/_padding.scss](../../src/utilities/_padding.scss)

## Variables

```sass
$zss--spacing-scale: 0 0.25rem 0.5rem 1rem 2rem 4rem !default;
```

All padding classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

The padding classes use the following naming scheme.

- just a number: padding on all sides
- t, r, b, l: top, right, bottom, left
- x: left and right
- y: top and bottom

For each value in `$zss--spacing-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated.

```css
.u-padding--1 { padding: 0.25rem; }
.u-padding--t1 { padding-top: 0.25rem; }
.u-padding--r1 { padding-right: 0.25rem; }
.u-padding--b1 { padding-bottom: 0.25rem; }
.u-padding--l1 { padding-left: 0.25rem; }

.u-padding--t1n { padding-top: -0.25rem; }
.u-padding--r1n { padding-right: -0.25rem; }
.u-padding--b1n { padding-bottom: -0.25rem; }
.u-padding--l1n { padding-left: -0.25rem; }

.u-padding--y1 {
    padding-top: 0.25rem;
    padding-bottom: 0.25rem
}
.u-padding--x1 {
    padding-right: 0.25rem;
    padding-left: 0.25rem
}

@media (min-width: 550px) {
    .u-padding--1\@sm { padding: 0.25rem; }
    .u-padding--t1\@sm { padding-top: 0.25rem; }
    .u-padding--r1\@sm { padding-right: 0.25rem; }
    .u-padding--b1\@sm { padding-bottom: 0.25rem; }
    .u-padding--l1\@sm { padding-left: 0.25rem; }

    .u-padding--t1n\@sm { padding-top: -0.25rem; }
    .u-padding--r1n\@sm { padding-right: -0.25rem; }
    .u-padding--b1n\@sm { padding-bottom: -0.25rem; }
    .u-padding--l1n\@sm { padding-left: -0.25rem; }
        
    .u-padding--y1\@sm {
        padding-top: 0.25rem;
        padding-bottom: 0.25rem
    }
    .u-padding--x1\@sm {
        padding-right: 0.25rem;
        padding-left: 0.25rem
    }
}
```

## Examples

```html
<div class="u-padding--1  u-padding--x2@lg  u-padding--y3@lg">
    On mobile, this element has a padding of 0.25rem on all sides.
    On desktop, this element has a padding of 0.5rem at the right and left, and a
        padding of 1rem on the top and bottom.
</div>
```

## References

- [MDN: padding](https://developer.mozilla.org/en/docs/Web/CSS/padding)
