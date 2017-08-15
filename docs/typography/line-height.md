# Line height

ZSS contains utility classes for setting values for the `line-height` property.

## Source files

- [utilities/_line-height.scss](../../src/utilities/_line-height.scss)

## Variables

```sass
$zss--line-height-scale: 0 1 1.25 1.5 1.75 !default;
```

All line height classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

For each value in `$zss--line-height-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-lh--0 { line-height: 0; }
.u-lh--1 { line-height: 1; }
.u-lh--2 { line-height: 1.25; }
.u-lh--3 { line-height: 1.5; }
.u-lh--4 { line-height: 1.75; }

@media (min-width: 550px) {
    .u-lh--0\@sm { line-height: 0; }
    .u-lh--1\@sm { line-height: 1; }
    .u-lh--2\@sm { line-height: 1.25; }
    .u-lh--3\@sm { line-height: 1.5; }
    .u-lh--4\@sm { line-height: 1.75; }
}
```

## Examples

```html
<h3 class="u-lh--1  u-lh--2@lg">Line height of 1 on mobile, line height of 2 on desktop.</h3>
```

## References

- [MDN: line-height](https://developer.mozilla.org/en/docs/Web/CSS/line-height)
