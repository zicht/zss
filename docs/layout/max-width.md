# Max-width

ZSS contains utility classes for setting values for the `max-width` property.

## Source files

- [utilities/_max-width.scss](../../src/utilities/_max-width.scss)

## Variables

```sass
$zss--max-width--scale: 1rem 2rem 4rem 8rem 16rem 32rem !default;
```

All max-width classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

For each value in `$zss--max-width--scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-width--mx1 { max-width: 1rem; }
.u-width--mx2 { max-width: 2rem; }
.u-width--mx3 { max-width: 4rem; }
.u-width--mx4 { max-width: 8rem; }
.u-width--mx5 { max-width: 16rem; }
.u-width--mx6 { max-width: 32rem; }

@media (min-width: 550px) {
    .u-width--mx1\@sm { max-width: 1rem; }
    .u-width--mx2\@sm { max-width: 2rem; }
    .u-width--mx3\@sm { max-width: 4rem; }
    .u-width--mx4\@sm { max-width: 8rem; }
    .u-width--mx5\@sm { max-width: 16rem; }
    .u-width--mx6\@sm { max-width: 32rem; }
}
```

Furthermore, there are a couple of classes that are not defined in variables.

```css
.u-width--mx100 { max-width: 100%; }
.u-width--mx-none { max-width: none; }

@media (min-width: 550px) {
    .u-width--mx100\@sm { max-width: 100%; }
    .u-width--mx-none\@sm { max-width: none; }
}
```

## Examples

```html
<section>
    <p class="u-width--mx5@lg">This paragraph has a max-width of 16 rem on desktop.</p>
</section>
```

## References

- [MDN: max-width](https://developer.mozilla.org/en/docs/Web/CSS/max-width)
