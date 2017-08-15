# Z-index

ZSS contains utility classes for setting values for the `z-index` property.

## Source files

- [utilities/_z-index.scss](../../src/utilities/_z-index.scss)

## Variables

ZSS has a fixed set of `z-index` values so there is no variable to configure.

The overflow classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the generated z-index classes.

```sass
.u-z--bottom { z-index: -1; }
.u-z--1 { z-index: 1; }
.u-z--2 { z-index: 2; }
.u-z--3 { z-index: 3; }
.u-z--4 { z-index: 4; }
.u-z--top { z-index: 666; }

@media (min-width: 550px) {
    .u-z--bottom\@sm { z-index: -1; }
    .u-z--1\@sm { z-index: 1; }
    .u-z--2\@sm { z-index: 2; }
    .u-z--3\@sm { z-index: 3; }
    .u-z--4\@sm { z-index: 4; }
    .u-z--top\@sm { z-index: 666; }
}
```

## Examples

```html
<div class="u-relative  u-z--1">
    <p>These elements are layered above other elements.</p>
</div>
```

## References

- [MDN: z-index](https://developer.mozilla.org/en/docs/Web/CSS/z-index)
