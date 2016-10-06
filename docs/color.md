# Colors

ZSS has support for utility classes that set text and background colors.

The default colors are:

- black: `#000`
- white: `#fff`
- transparent: `transparent`

## Customizing

The variable `$zss--colors` is a Sass map (dictionary). The key is used in the generated class name, while the value should be a color value that's understood by CSS (hex, rgb, et cetera).

You can add your own colors to the map:

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