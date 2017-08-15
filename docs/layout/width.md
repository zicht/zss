# Width

ZSS contains utility classes for setting values for the `width` property.

## Source files

- [utilities/_width.scss](../../src/utilities/_width.scss)

## Variables

```sass
$zss--width--scale: 1rem 2rem 4rem 8rem !default;
$zss--width--percentage-scale: 10 20 25 33 50 66 75 100 !default;
```

All width classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

For each value in `$zss--width--scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-width--1 { width: 1rem; }
.u-width--2 { width: 2rem; }
.u-width--3 { width: 4rem; }
.u-width--4 { width: 8rem; }

@media (min-width: 550px) {
    .u-width--1\@sm { width: 1rem; }
    .u-width--2\@sm { width: 2rem; }
    .u-width--3\@sm { width: 4rem; }
    .u-width--4\@sm { width: 8rem; }
}
```

For each value in `$zss--width--percentage-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-width--10 { width: 10%; }
.u-width--20 { width: 20%; }
.u-width--25 { width: 25%; }
.u-width--33 { width: 33%; }
.u-width--50 { width: 50%; }
.u-width--66 { width: 66%; }
.u-width--75 { width: 75%; }
.u-width--100 { width: 100%; }

@media (min-width: 550px) {
    .u-width--10\@sm { width: 10%; }
    .u-width--20\@sm { width: 20%; }
    .u-width--25\@sm { width: 25%; }
    .u-width--33\@sm { width: 33%; }
    .u-width--50\@sm { width: 50%; }
    .u-width--66\@sm { width: 66%; }
    .u-width--75\@sm { width: 75%; }
    .u-width--100\@sm { width: 100%; }
}
```

Furthermore, there are a couple of classes that are not defined in variables.

```css
.u-width--auto { width: auto; }
.u-width--100v { width: 100vw; }

@media (min-width: 550px) {
    .u-width--auto\@sm { width: auto; }
    .u-width--100v\@sm { width: 100vw; }
}
```

## Examples

```html
<section>
    <div class="u-width--50@lg">This element has a width of 50% of its parent on desktop.</div>
</section>
```

## References

- [MDN: width](https://developer.mozilla.org/en/docs/Web/CSS/width)
