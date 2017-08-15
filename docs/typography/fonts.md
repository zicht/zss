# Fonts

ZSS contains utility classes for setting font properties.

## Source files

- [utilities/_font-size.scss](../../src/utilities/_font-size.scss)
- [utilities/_font-style.scss](../../src/utilities/_font-style.scss)
- [utilities/_font-variant.scss](../../src/utilities/_font-variant.scss)
- [utilities/_font-weight.scss](../../src/utilities/_font-weight.scss)

## Variables

The values for `font-size` are defined in `$zss--type-scale`.

```sass
$zss--type-scale: 6rem 4rem 3rem 2rem 1.5rem 1rem 0.75rem 0.5rem !default;
```

## Generated CSS

### `font-size`

For each color in `$zss--type-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-size--1 { font-size: 6rem; }
.u-size--2 { font-size: 4rem; }
.u-size--3 { font-size: 3rem; }
.u-size--4 { font-size: 2rem; }
.u-size--5 { font-size: 1.5rem; }
.u-size--6 { font-size: 1rem; }
.u-size--7 { font-size: .75rem; }
.u-size--8 { font-size: .5rem; }

@media (min-width: 550px) {
    .u-size--1\@sm { font-size: 6rem; }
    .u-size--2\@sm { font-size: 4rem; }
    .u-size--3\@sm { font-size: 3rem; }
    .u-size--4\@sm { font-size: 2rem; }
    .u-size--5\@sm { font-size: 1.5rem; }
    .u-size--6\@sm { font-size: 1rem; }
    .u-size--7\@sm { font-size: .75rem; }
    .u-size--8\@sm { font-size: .5rem; }
}
```

### `font-style`

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-italic { font-style: italic; }

@media (min-width: 550px) {
    .u-italic\@sm { font-style: italic; }
}
```

### `font-variant`

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-small-caps { font-variant: small-caps; }

@media (min-width: 550px) {
    .u-small-caps\@sm { font-variant: small-caps; }
}
```

### `font-weight`

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-weight--100 { font-weight: 100; }
.u-weight--200 { font-weight: 200; }
.u-weight--300 { font-weight: 300; }
.u-weight--400 { font-weight: 400; }
.u-weight--500 { font-weight: 500; }
.u-weight--600 { font-weight: 600; }
.u-weight--700 { font-weight: 700; }
.u-weight--800 { font-weight: 800; }
.u-weight--900 { font-weight: 900; }

@media (min-width: 550px) {
    .u-weight--100\@sm { font-weight: 100; }
    .u-weight--200\@sm { font-weight: 200; }
    .u-weight--300\@sm { font-weight: 300; }
    .u-weight--400\@sm { font-weight: 400; }
    .u-weight--500\@sm { font-weight: 500; }
    .u-weight--600\@sm { font-weight: 600; }
    .u-weight--700\@sm { font-weight: 700; }
    .u-weight--800\@sm { font-weight: 800; }
    .u-weight--900\@sm { font-weight: 900; }
}
```

## Examples

```html
<p class="u-size--1  u-size--4@lg">Big text on mobile, smaller text on desktop.</p>

<p class="u-italic@md">Italic text on desktop.</p>

<p class="u-small-caps@md">Small caps on desktop.</p>

<p class="u-weight--400  u-weight--700@md">Normal text on mobile, bold text on desktop.</p>
```

## References

- [MDN: font-size](https://developer.mozilla.org/en/docs/Web/CSS/font-size)
- [MDN: font-style](https://developer.mozilla.org/en/docs/Web/CSS/font-style)
- [MDN: font-variant](https://developer.mozilla.org/en/docs/Web/CSS/font-variant)
- [MDN: font-weight](https://developer.mozilla.org/en/docs/Web/CSS/font-weight)
