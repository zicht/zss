# Backgrounds

ZSS contains utility classes for setting CSS properties concerning background images.

## Source files

- [utilities/_background-position.scss](../../src/utilities/_background-position.scss)
- [utilities/_background-repeat.scss](../../src/utilities/_background-repeat.scss)
- [utilities/_background-size.scss](../../src/utilities/_background-size.scss)

## Variables

Since the background CSS properties have a fixed set of values, there is no variable to configure.   

The background classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the background classes that are generated.

`background-position`:

```css
.u-bg--top { background-position: top; }
.u-bg--right { background-position: right; }
.u-bg--bottom { background-position: bottom; }
.u-bg--left { background-position: left; }
.u-bg--center { background-position: center; }

@media (min-width: 550px) {
    .u-bg--top\@sm { background-position: top; }
    .u-bg--right\@sm { background-position: right; }
    .u-bg--bottom\@sm { background-position: bottom; }
    .u-bg--left\@sm { background-position: left; }
    .u-bg--center\@sm { background-position: center; }
}
```

`background-repeat`:

```css
.u-bg--repeat { background-repeat: repeat; }
.u-bg--repeat-x { background-repeat: repeat-x; }
.u-bg--repeat-y { background-repeat: repeat-y; }
.u-bg--no-repeat { background-repeat: no-repeat; }

@media (min-width: 550px) {
    .u-bg--repeat\@sm { background-repeat: repeat; }
    .u-bg--repeat-x\@sm { background-repeat: repeat-x; }
    .u-bg--repeat-y\@sm { background-repeat: repeat-y; }
    .u-bg--no-repeat\@sm { background-repeat: no-repeat; }
}
```

`background-size`:

```css
.u-bg--contain { background-size: contain; }
.u-bg--cover { background-size: cover; }

@media (min-width: 550px) {
    .u-bg--contain\@sm { background-size: contain }
    .u-bg--cover\@sm { background-size: cover }
}
```

## Examples

```html
<div class="u-bg--cover  u-bg--no-repeat" style="background-image: url(../image.webp)">
    <p>Text with a single background image.</p>
</div>
```

## References

- [MDN: background-position](https://developer.mozilla.org/en/docs/Web/CSS/background-position)
- [MDN: background-repeat](https://developer.mozilla.org/en/docs/Web/CSS/background-repeat)
- [MDN: background-size](https://developer.mozilla.org/en/docs/Web/CSS/background-size)
