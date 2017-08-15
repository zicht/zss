# Display

ZSS contains utility classes for setting values for the `display` property.

## Source files

- [utilities/_display.scss](../../src/utilities/_display.scss)

## Variables

Since `display` has a fixed set of values, there is no variable to configure. 

The display classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the display classes that are generated.

```sass
.u-hidden { display: none; }
.u-block { display: block; }
.u-inline { display: inline; }
.u-inline-block { display: inline-block; }
.u-flex { display: flex; }
.u-flex--inline { display: inline-flex; }
.u-table { display: table; }
.u-cell { display: table-cell; }
.u-row { display: table-row; }
.u-row-group { display: table-row-group; }
.u-column { display: table-column; }
.u-column-group { display: table-column-group; }

@media (min-width: 550px) {
    .u-hidden\@sm { display: none; }
    .u-block\@sm { display: block; }
    .u-inline\@sm { display: inline; }
    .u-inline-block\@sm { display: inline-block; }
    .u-flex\@sm { display: flex; }
    .u-flex--inline\@sm { display: inline-flex; }
    .u-table\@sm { display: table; }
    .u-cell\@sm { display: table-cell; }
    .u-row\@sm { display: table-row; }
    .u-row-group\@sm { display: table-row-group; }
    .u-column\@sm { display: table-column; }
    .u-column-group\@sm { display: table-column-group; }
}
```

## Examples

```html
<div class="u-hidden  u-block@sm">
    <p>This element is hidden on mobile and visible on bigger screens.</p>
</div>
```

## References

- [MDN: display](https://developer.mozilla.org/en/docs/Web/CSS/display)
