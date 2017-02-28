# Colors

ZSS contains utility classes for setting text and background colors. It does not come with any defined colors except for
black, white and transparent.

## Referenced files

- [utilities/_background-color.scss](../../src/utilities/_background-color.scss)
- [utilities/_color.scss](../../src/utilities/_color.scss)

## Variables

```
$zss--colors: (
    black: #000,
    white: #fff,
    transparent: transparent
) !default;
```

- The key is used in the generated class name. 
- The value can be any color format that's understood by CSS (hexadecimal, RGB, HSL et cetera).

The color classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS classes

Below is an example of the color classes that are generated for a single color, for both text and background.

`color`:

```
.u-black { color: #000 }
.u-hover--black:hover { color: #000 }

@media (min-width: 550px) {
    .u-black\@sm { color: #000 }
    .u-hover--black\@sm:hover { color: #000 }
}
```

`background-color`:

```
.u-bg--black { background-color: #000 }
.u-bg--hover--black:hover { background-color: #000 }

@media (min-width: 550px) {
    .u-bg--black\@sm { background-color: #000 }
    .u-bg--hover--black\@sm:hover { background-color: #000 }
}
```


## Customizing

If you want to include the three default colors of ZSS, you can add your own colors to the map:

```
$zss--colors: map-merge(
    $zss--colors, (
        'red': #f90,
        'orange': #f09;
    )
);
```

Alternatively, if you don't want to include the default colors, just override the variable entirely:

```
$zss--colors: (
    'red': #f90,
    'orange': #f09;
);
```
