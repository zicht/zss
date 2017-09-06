# Unit helpers

ZSS provides functions for dealing with value units.

## Source files

- [helpers/_units.scss](../../src/helpers/_units.scss)

## Functions

### `rem`  

~~Generates 90's pop music~~ Transforms the given pixel value
into a value based on the `rem` unit.

#### Parameters

- `$px`   
   A pixel value, e.g. `16px`.

### `strip-units`

Removes the unit from the given value.

#### Parameters

- `$value`   
   A value with an optional unit, that will be removed if present.

## Examples

```sass
.hodor {
    font-size: rem(16px);
}

.art-vandelay {
    line-height: strip-units(1rem); // line-height: 1
}
```
