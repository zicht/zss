# Changelog

## Version 2.0

An extensive cleanup and a lot of new utility classes 🎉

### Development checks

`~/dev/_strict.scss` contains sanity checks that give compiler warnings and errors if your variable scales are not correct, or if you use values that don’t make sense from a design perspective.

### Refactoring variables

Variables were spread across several files. `_responsive.scss` contained responsive variables, `_grid.scss` contained grid variables et cetera. Not anymore: all configurable ZSS variables can be found in one file: `_zss-defaults.scss`.

Furthermore: variables are named more consistently. Now, each variable starts with a `$zss--` prefix and they better reflect what's in them.

And lastly: most configurable properties are now based on a scale. For example, there is a variable `$zss--line-height-scale`. This should keep the number of values used for a property in check.

### Removed `flex-with-fallback` grid type

The fallback grid type proved too buggy to be useful, so there are now only two types of grid: `flex` (the default) and `float`.

### Added the `o-media` object

A flex implementation of the famous [media object](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/) for the very common UI pattern of positioning an image next to a bunch of text.

### Changed color structure

Previously, colors were defined twice: both separate variables and a Sass map for generating utility classes. This was unnecessary and prone to errors.
Now there are no more color variables: every color is defined directly in the map.

```
$zss--colors: (
    black: #000,
    white: #fff,
    transparent: transparent
)
```

You're strongly encouraged to use the generated utility classes if you need to add a color to your component, but if you really do need to access a color you can use the new mixin `color`:

```
.x {
    color: color(black);
}
```

Also, it's now possible to automatically generated lighter variations of color with the `zss--color-opacity-scale`. By default, it takes the color map and generates variations with 0.25, 0.5 and 0.75 opacity.

### New utility classes and a bit of refactoring

Each CSS property now has it's own file, so it's easier to find in which file a property is located. Also: every utility class is now responsive, if applicable. (For example, the cursor is not responsive.)

These properties where added as a utility class:

- `background-size`
- `border-color`
- `border-radius`
- `border-style`
- `border-width`
- `cursor`
- `font-size`
- `font-weight`
- `height`
- `line-height`
- `max-width`
- `min-height`
- `vertical-align`
- `width`
- `z-index`

These properties were expanded or changed:

- Added a hover class for each color.
- Added much more flex properties.
- Added color variations with an opacity scale.
- Margin and padding are moved from `_whitespace.scss` to two separate files.
- The overflow classes are renamed from `u-overflow` to `u-of`.
- The float classes renamed. For example, `u-left` is renamed to `u-f--left`.

### Several minor tweaks

- `o-ui-list` is renamed to `o-list-reset`.
- Added a `strip-units` mixin for removing the unit part of a Sass string.
- Added a `hover` mixin for easily applying hover/active/focus states.
- Removed the `font-rem` mixin. Use a utility class from the line height scale instead.
- Removed  the `z-index` mixin in favour of the z-index utility classes.
- Updated the included [normalize.css](http://necolas.github.io/normalize.css/) from v3.0.3 to v5.0.0.
- Changed the base font size from `18px` to `1rem`.
- Changed the base line height from `26px` to `1.5`.

## Version 1.0

Initial version.
