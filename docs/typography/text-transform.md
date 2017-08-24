# Text transform

ZSS contains utility classes for setting values for the `text-transform` property.

## Source files

- [utilities/_text-transform.scss](../../src/utilities/_text-transform.scss)

## Generated CSS

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-capitalize { text-transform: capitalize; }
.u-lower { text-transform: lowercase; }
.u-upper { text-transform: uppercase; }
.u-no-transform { text-transform: none; }

@media (min-width: 550px) {
    .u-capitalize\@sm { text-transform: capitalize; }
    .u-lower\@sm { text-transform: lowercase; }
    .u-upper\@sm { text-transform: uppercase; }
    .u-no-transform\@sm { text-transform: none; }
}
```
## Examples

```html
<p class="u-upper  u-no-transform@lg">Uppercase text on mobile, default text on desktop.</p>
```

## References

- [MDN: text-transform](https://developer.mozilla.org/en/docs/Web/CSS/text-transform)
