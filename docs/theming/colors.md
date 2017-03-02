# Colors

ZSS contains utility classes for setting text and background colors. It does not come with any defined colors except for
black, white and transparent.

## Source files

- [utilities/_background-color.scss](../../src/utilities/_background-color.scss)
- [utilities/_color.scss](../../src/utilities/_color.scss)

## Variables

```sass
$zss--colors: (
    black: #000,
    white: #fff,
    transparent: transparent
) !default;
```

- The key is used in the generated class name. 
- The value can be any color format that's understood by CSS (hexadecimal, RGB, HSL et cetera).

The color classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the color classes that are generated for a single color, for both text and background.

`color`:

```sass
.u-black { color: #000 }
.u-hover--black:hover { color: #000 }

@media (min-width: 550px) {
    .u-black\@sm { color: #000 }
    .u-hover--black\@sm:hover { color: #000 }
}
```

`background-color`:

```sass
.u-bg--black { background-color: #000 }
.u-bg--hover--black:hover { background-color: #000 }

@media (min-width: 550px) {
    .u-bg--black\@sm { background-color: #000 }
    .u-bg--hover--black\@sm:hover { background-color: #000 }
}
```


## Customizing

If you want to include the three default colors of ZSS, you can add your own colors to the map:

```sass
$zss--colors: map-merge(
    $zss--colors, (
        'red': #f90,
        'orange': #f09;
    )
);
```

Alternatively, if you don't want to include the default colors, just override the variable entirely:

```sass
$zss--colors: (
    'red': #f90,
    'orange': #f09;
);
```

## Examples

Given the variable `$zss--colors` contains `black` and `white`.

```html
<p class="u-bg--black  u-white">
    White text on a black background.
</p>

<p> class="u-white  u-black@md">
    White text on small screens, black text from the `md` breakpoint up.
</p>
```

## References

- [MDN: background-color](https://developer.mozilla.org/en/docs/Web/CSS/background-color)
- [MDN: color](https://developer.mozilla.org/en/docs/Web/CSS/color)
