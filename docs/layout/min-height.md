# Min-height

ZSS contains utility classes for setting values for the `min-height` property.

## Source files

- [utilities/_min-height.scss](../../src/utilities/_min-height.scss)

## Variables

The min-height classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the classes that are generated.

```sass
.u-height--m100 { min-height: 100%; }

@media (min-width: 550px) {
    .u-height--m100\@sm { min-height: 100%; }
}
```

## Examples

```html
<div class="u-height--m100@lg">
    <p>This element has a minimal height of 100% on bigger screens.</p>
</div>
```

## References

- [MDN: min-height](https://developer.mozilla.org/en/docs/Web/CSS/min-height)
