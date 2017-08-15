# Opacity

ZSS contains utility classes for setting values for the `opacity` property.

## Source files

- [utilities/_opacity.scss](../../src/utilities/_opacity.scss)

## Variables

```sass
$zss--color-opacity-scale: 0 0.25 0.5 0.75 1 !default;
```

All opacity classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

For each value in `$zss--color-opacity-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-opacity--0 { opacity: 0; }
.u-opacity--25 { opacity: .25; }
.u-opacity--50 { opacity: .5; }
.u-opacity--75 { opacity: .75; }
.u-opacity--100 { opacity: 1; }

@media (min-width: 550px) {
    .u-opacity--0\@sm { opacity: 0; }
    .u-opacity--25\@sm { opacity: .25; }
    .u-opacity--50 { opacity: .5; }
    .u-opacity--75\@sm { opacity: .75; }
    .u-opacity--100\@sm { opacity: 1; }
}
```

## Examples

```html
<div class="u-bg--black">
    <p class="u-opacity--100  u-opacity--50@lg  u-white">This element has white text on mobile, and 50% transparent white on desktop.</p>
</div>
```

## References

- [MDN: opacity](https://developer.mozilla.org/en/docs/Web/CSS/opacity)
