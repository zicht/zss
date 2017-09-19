# Object-fit

ZSS contains utility classes for setting values for the CSS property `object-fit`.

## Source files

- [utilities/_object-fit.scss](../../src/utilities/_object-fit.scss)

## Variables

Since the `object-fit` property has a fixed set of values, there is no variable to configure.   

The classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the classes that are generated.

`object-fit`:

```css
.u-fit--fill { object-fit: fill; }
.u-fit--contain { object-fit: contain; }
.u-fit--cover { object-fit: cover; }
.u-no-fit { object-fit: none; }

@media (min-width: 550px) {
    .u-fit--fill\@sm { object-fit: fill; }
    .u-fit--contain\@sm { object-fit: contain; }
    .u-fit--cover\@sm { object-fit: cover; }
    .u-no-fit\@sm { object-fit: none; }
}
```

## Examples

```html
<figure>
    <img src="image.webp" class="u-fit--cover">
    <figcaption>Image that covers the element’s content box, similar to `background-size: cover`.</figcaption>
</figure>
```

## References

- [MDN: object-fit](https://developer.mozilla.org/en/docs/Web/CSS/object-fit)
