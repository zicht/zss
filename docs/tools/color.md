# Color helper

ZSS provides a mixin `get-color` to help access colors defined in `$zss--colors`. The mixin throws
an error if it cannot find the requested color in `$zss--colors`. This can help to make sure
no other colors are used.

## Source files

- [helpers/_color.scss](../../src/helpers/_color.scss)

## Functions

### `get-color`  

Retrieves a color value from the pre-defined Sass map `$zss--colors`.

#### Parameters

- `$name`   
   A string representing the name of a color defined in `$zss--colors`.

## Examples

```sass
.hodor {
    background-color: get-color(blue--cerulean);
}
```