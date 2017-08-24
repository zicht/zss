# Text decoration

ZSS contains utility classes for setting values for the `text-decoration` property.

## Source files

- [utilities/_text-decoration.scss](../../src/utilities/_text-decoration.scss)

## Generated CSS

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```css
.u-strike { text-decoration: line-through; }
.u-underline { text-decoration: underline; }
.u-no-decoration { text-decoration: none; }

@media (min-width: 550px) {
    .u-strike\@sm { text-decoration: line-through; }
    .u-underline\@sm { text-decoration: underline; }
    .u-no-decoration\@sm { text-decoration: none; }
}
```
## Examples

```html
<a href="#" class="u-no-decoration">This link has no underline.</a>
```

## References

- [MDN: text-decoration](https://developer.mozilla.org/en/docs/Web/CSS/text-decoration)
