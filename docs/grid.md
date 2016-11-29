# Grid

The ZSS rid object is a way to align your components onto a view, similar to the well-known Bootstrap grid.

## Using the grid

1. Create a grid container.
2. Add a row that will contain your columns.
3. Add one or more columns to the row.

### The grid container

The grid container is the wrapper for your entire grid.

- Use the class `o-grid` if you want a fluid grid that spans the entire width of the viewport.
- Add the modifier `o-grid--fixed` for a grid with a fixed max-width on each breakpoint.
- Add the modifier `o-grid--flex-content` if you want each column to have `display: flex` applied. With this modifier, the content you add to the columns can be aligned with flexbox.

### Grid rows

Grid rows divide the page into vertical sections. Use as many as you like inside a container. Just add the class `o-grid__row` to a child element of the grid container.

### Grid colums

Grid columns divide the page into horizontal sections. They work by specifying how many of the maximum available columns you want your element to span, at which breakpoint.

1. Add the class `o-grid__col` to one ore more columns.
2. Add a class that defines the width of the column. Examples: `o-grid__col--12@xs`, `o-grid__col--6@md`.

## Customizing

### Width

When the grid is not fluid, the grid applies several `max-width` values at certain breakpoints. Override the variables `$zss--grid-max-widths` to modify these values. The default values are:

```
$zss--grid-max-widths: (
    sm: 530px,
    md: 750px,
    lg: 960px,
    xl: 1170px
) !default;
```

### Number of columns

The default number of columns is 12. If your content requires fewer or more columns, override the variable `$zss--grid-columns`.

### Gutter

The default gutter width between the columns is `2rem`. Override the variable `$zss--grid-gutter` if you require a different value.

### Grid type

Grid columns are typically constructed with floats. However, the flexbox model makes building grids easier, especially if you want the columns in a row to have an equal height. One drawback is that the [browser support for flexbox](http://caniuse.com/#search=flexbox) is less favourable, but it's still acceptable, though.

You can choose the type of grid you want. The variable `$zss--grid-type` has these possible values:
1. `$zss--grid-type: flex` (default)   
The grid is generated with flexbox properties. Use this if you work with modern browsers.
2. `$zss--grid-type: float`   
The grid is generated with floats (the old Bootstrap way). Use this if you need support for older browsers, and don't require columns of equal height.