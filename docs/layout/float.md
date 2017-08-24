# Float

ZSS contains utility classes for setting values for the `float` property.

## Source files

- [utilities/_float.scss](../../src/utilities/_float.scss)

## Variables

Since the float CSS properties have a fixed set of values, there is no variable to configure.   

The float classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the float classes that are generated.

```sass
.u-f--right { float: right; }
.u-f--left { float: left; }
.u-f--none { float: none; }

@media (min-width: 550px) {
    .u-f--right\@sm { float: right; }
    .u-f--left\@sm { float: left; }
    .u-f--none\@sm { float: none; }
}
```

## Examples

```html
<div class="u-f--left  u-f--none@sm">
    This element floats to the left on mobile, but not on bigger screens.
</div>
```

## References

- [MDN: float](https://developer.mozilla.org/en/docs/Web/CSS/float)
