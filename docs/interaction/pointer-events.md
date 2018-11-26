# Pointer events

ZSS contains utility classes for setting values for the `pointer-events` property.

## Source files

- [utilities/_pointer-events.scss](../../src/utilities/_pointer-events.scss)

## Variables

Since the pointer events have a fixed set of values, there is no variable to configure.   

## Generated CSS

Below is an example of the pointer events classes that are generated.

```css
.u-events--auto { pointer-events: auto; }
.u-events--none { pointer-events: none; }
```

## Examples

```html
<button class="u-events--none">
    Nothing happens when this button is clicked.
</button>
```

## References

- [MDN: pointer-events](https://developer.mozilla.org/en-US/docs/Web/CSS/pointer-events)
