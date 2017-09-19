# Text decoration skip

ZSS contains utility classes for setting a value for the `text-decoration-skip` property.

## Source files

- [utilities/_text-decoration-skip.scss](../../src/utilities/_text-decoration-skip.scss)

## Generated CSS

This property has no responsive classes, since a scenario where the text-decoration should
be skipped on only a few devices is not very likely.

```css
.u-skip--ink { text-decoration-skip: ink; }
.u-no-skip { text-decoration-skip: none; }
```
## Examples

```html
<a href="#" class="u-underline  u-skip--ink">
    This link has an underline, with no glyphs that are touched by the underline.
</a>
```

## References

- [MDN: text-decoration-skip](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-skip)
