# Grid helpers

ZSS uses several mixins to generate grid classes. These mixins are available
if you would like to generate a grid with different class names.

## Source files

- [helpers/_grid.scss](../../src/helpers/_grid.scss)

## Mixins

### `create-grid`  

Generates code for a grid container.

#### Parameters

- `$gutter`   
   The width between grid columns. Must be an integer with a valid CSS unit, e.g. `18px` or `2rem`.

### `create-grid-widths`

Generates max-width CSS that can be used for grids that have a fixed max width at certain breakpoints.

#### Parameters

- `$max-widths`   
  A Sass map containing the max-width of the grid per breakpoint. The key is the name of the breakpoint 
  and must correspond to a valid breakpoint name, as defined in the `$breakpoints` parameter.
  The value must be valid for `max-width`.
- `$breakpoints`   
  A Sass map containing the breakpoints at which the width of the grid changes. The key is the name of 
  the breakpoint; the value is a valid device width.

### `create-grid-row`  

Generates a grid row.

#### Parameters

- `$gutter`   
   The width between grid columns. Must be an integer with a valid CSS unit, e.g. `18px` or `2rem`.

### `create-grid-column`  

Generates a base for a grid column.

#### Parameters

- `$gutter`   
   The width between grid columns. Must be an integer with a valid CSS unit, e.g. `18px` or `2rem`.

### `create-grid-column-sizes`  

Generates column classes to be able to change the width of a column across breakpoints.

#### Parameters

- `$column-count`   
  An integer that defines how many columns the grid can contain.
- `$breakpoints`   
  A Sass map containing the breakpoints at which columns change width. The key is the name of 
  the breakpoint; the value is a valid device width.

### `create-grid-column-offset`  

Generates column offset classes to be able to push columns to the right across breakpoints.

#### Parameters

- `$column-count`   
  An integer that defines how many columns the grid can contain.
- `$breakpoints`   
  A Sass map containing the breakpoints at which columns change width. The key is the name of 
  the breakpoint; the value is a valid device width.

## Examples

```sass
.widths {
    @include create-grid-widths(
        (
            'tablet': 800px
            'desktop': 1024px,
            'tv': 1400px
        ),
        (
            'tablet': 1024px,
            'desktop': 1400px,
            'tv': '1800px
        )
    );
}
```
