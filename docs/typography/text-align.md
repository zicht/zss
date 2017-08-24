# Text align

ZSS contains utility classes for setting values for the `text-align` property.

## Source files

- [utilities/_text-align.scss](../../src/utilities/_text-align.scss)

## Generated CSS

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-text--right { text-align: right; }
.u-text--center { text-align: center; }
.u-text--left { text-align: left; }

@media (min-width: 550px) {
    .u-text--right\@sm { text-align: right; }
    .u-text--center\@sm { text-align: center; }
    .u-text--left\@sm { text-align: left; }
}
```
## Examples

```html
<p class="u-text--center  u-text--right@lg">This text is centered on small devices, and aligned right on bigger screens.</p>
```

## References

- [MDN: text-align](https://developer.mozilla.org/en/docs/Web/CSS/text-align)
