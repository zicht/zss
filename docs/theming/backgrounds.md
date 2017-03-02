# Backgrounds

ZSS contains utility classes for setting CSS properties concerning background images.

## Source files

- [utilities/_background-size.scss](../../src/utilities/_background-size.scss)

## Variables

Since the background CSS properties have a fixed set of values, there is no variable to configure.   

The background classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the background classes that are generated.

`background-size`:

```sass
.u-bg--contain { background-size: contain; }
.u-bg--cover { background-size: cover; }

@media (min-width: 550px) {
    .u-bg--contain\@sm { background-size: contain }
    .u-bg--cover\@sm { background-size: cover }
}
```

## Examples

```html
<div class="u-bg--cover" style="background-image: url(../images.webp)">
    <p>Text with background image.</p>
</div>
```

## References

- [MDN: background-size](https://developer.mozilla.org/en/docs/Web/CSS/background-size)
