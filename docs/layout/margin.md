# Margin

ZSS contains utility classes for setting values for the `margin` property.

## Source files

- [utilities/_margin.scss](../../src/utilities/_margin.scss)

## Variables

```sass
$zss--spacing-scale: 0 0.25rem 0.5rem 1rem 2rem 4rem !default;
```

All margin classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

The margin classes use the following naming scheme.

- just a number: margin on all sides
- t, r, b, l: top, right, bottom, left
- x: left and right
- y: top and bottom
- n: negative margin value

For each value in `$zss--spacing-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated.

```css
.u-margin--1 { margin: 0.25rem; }
.u-margin--t1 { margin-top: 0.25rem; }
.u-margin--r1 { margin-right: 0.25rem; }
.u-margin--b1 { margin-bottom: 0.25rem; }
.u-margin--l1 { margin-left: 0.25rem; }

.u-margin--t1n { margin-top: -0.25rem; }
.u-margin--r1n { margin-right: -0.25rem; }
.u-margin--b1n { margin-bottom: -0.25rem; }
.u-margin--l1n { margin-left: -0.25rem; }

.u-margin--y1 {
    margin-top: 0.25rem;
    margin-bottom: 0.25rem
}
.u-margin--x1 {
    margin-right: 0.25rem;
    margin-left: 0.25rem
}

@media (min-width: 550px) {
    .u-margin--1\@sm { margin: 0.25rem; }
    .u-margin--t1\@sm { margin-top: 0.25rem; }
    .u-margin--r1\@sm { margin-right: 0.25rem; }
    .u-margin--b1\@sm { margin-bottom: 0.25rem; }
    .u-margin--l1\@sm { margin-left: 0.25rem; }

    .u-margin--t1n\@sm { margin-top: -0.25rem; }
    .u-margin--r1n\@sm { margin-right: -0.25rem; }
    .u-margin--b1n\@sm { margin-bottom: -0.25rem; }
    .u-margin--l1n\@sm { margin-left: -0.25rem; }
        
    .u-margin--y1\@sm {
        margin-top: 0.25rem;
        margin-bottom: 0.25rem
    }
    .u-margin--x1\@sm {
        margin-right: 0.25rem;
        margin-left: 0.25rem
    }
}
```

Furthermore, there are a couple of classes with fixed values. They can be used for centering or positioning elements inside a flex container.

```css
.u-margin--t-auto { margin-top: auto; }
.u-margin--r-auto { margin-right: auto; }
.u-margin--b-auto { margin-bottom: auto; }
.u-margin--l-auto { margin-left: auto; }
.u-margin--x-auto {
    margin-right: auto;
    margin-left: auto;
}
.u-margin--y-auto {
    margin-top: auto;
    margin-bottom: auto;
}

@media (min-width: 550px) {
    .u-margin--t-auto\@sm { margin-top: auto; }
    .u-margin--r-auto\@sm { margin-right: auto; }
    .u-margin--b-auto\@sm { margin-bottom: auto; }
    .u-margin--l-auto\@sm { margin-left: auto; }
    .u-margin--x-auto\@sm {
        margin-right: auto;
        margin-left: auto;
    }
    .u-margin--y-auto\@sm {
        margin-top: auto;
        margin-bottom: auto;
    }
}
```

## Examples

```html
<div class="u-margin--1  u-margin--x2@lg  u-margin--y3@lg">
    On mobile, this element has a margin of 0.25rem on all sides.
    On desktop, this element has a margin of 0.5rem at the right and left, and a
        margin of 1rem on the top and bottom.
</div>
```

## References

- [MDN: margin](https://developer.mozilla.org/en/docs/Web/CSS/margin)
