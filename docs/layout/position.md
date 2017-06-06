# Position

ZSS contains utility classes for setting `position` and related CSS properties.

## Source files

- [utilities/_position.scss](../../src/utilities/_position.scss)

## Variables

Since the position CSS properties have a fixed set of values, there is no variable to configure. 
The `top`, `right`, `bottom` and `left` properties are included in this file as well, since they're
very much related.

The position classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the position classes that are generated.

```sass
.u-absolute { position: absolute; }
.u-fixed { position: fixed; }
.u-relative { position: relative; }
.u-static { position: static; }

.u-top--0 { top: 0; }
.u-right--0 { right: 0; }
.u-bottom--0 { bottom: 0; }
.u-left--0 { left: 0; }

@media (min-width: 550px) {
    .u-absolute\@sm { position: absolute; }
    .u-fixed\@sm { position: fixed; }
    .u-relative\@sm { position: relative; }
    .u-static\@sm { position: static; }

    .u-top--0\@sm { top: 0; }
    .u-right--0\@sm { right: 0; }
    .u-bottom--0\@sm { bottom: 0; }
    .u-left--0\@sm { left: 0; }
}
```

## Examples

```html
<div class="u-absolute@sm  u-bottom--0@sm">
    <p>This element is positioned in an absolute way to the bottom.</p>
</div>
```

## References

- [MDN: position](https://developer.mozilla.org/en/docs/Web/CSS/position)
- [MDN: top](https://developer.mozilla.org/en/docs/Web/CSS/top)
- [MDN: right](https://developer.mozilla.org/en/docs/Web/CSS/right)
- [MDN: bottom](https://developer.mozilla.org/en/docs/Web/CSS/bottom)
- [MDN: left](https://developer.mozilla.org/en/docs/Web/CSS/left)
