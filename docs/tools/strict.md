## Strict

Importing `dev/strict` will check your configuration for design smells and configuration errors at compile time.

## Source files

- [dev/_strict.scss](../../src/dev/_strict.scss)

## Performed checks

### Borders

- `$zss--border-radius-scale` should contain no more than 5 values.
- The values of `$zss--border-radius-scale` must be sorted in a ascending order.
- `$zss--border-width-scale` should contain no more than 5 values.
- The values of `$zss--border-width-scale` must be sorted in a ascending order.
- The values of `$zss--border-colors` must be defined in `$zss--colors`.

## Dimensions

- The values of `$zss--width-scale` must be sorted in a ascending order.
- The values of `$zss--width--percentage-scale` must be sorted in a ascending order.
- The values of `$zss--max-width-scale` must be sorted in a ascending order.
- The values of `$zss--height-scale` must be sorted in a ascending order.
- The values of `$zss--height--percentage-scale` must be sorted in a ascending order.

### Objects

- The value of `$zss--grid-gutter` must be defined in `$zss--spacing-scale`.
- The value of `$zss--media-margin` must be defined in `$zss--spacing-scale`.

### Typography

- `$zss--type-scale` should contain no more than 8 values.
- The values of `$zss--type-scale` must be sorted in a descending order.
- The value of `$zss--base-font-size` must be defined in `$zss--type-scale`.
- `$zss--line-height-scale` should contain no more than 5 values.
- The values of `$zss--line-height-scale` must be sorted in a ascending order.
- The value of `$zss--base-line-height` must be defined in `$zss--line-height-scale`.

### Whitespace

- `$zss--spacing-scale` should contain no more than 8 values.
- The values of `$zss--spacing-scale` must be sorted in a ascending order.
