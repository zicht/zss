# Clear

ZSS contains a few utility classes for clearing floats.

## Source files

- [helpers/_clear.scss](../../src/helpers/_clear.scss)
- [utilities/_clear.scss](../../src/utilities/_clear.scss)

## Generated CSS

Use `.u-clear--inside` to clear floats that are inside the element to which this class is applied. (It uses the clearfix construct from [@necolas](https://github.com/necolas).)

```sass
.u-clear--inside::before,
.u-clear--inside::after {
    display: table;
    content: ' ';
}

.u-clear--inside::after { clear: both; }
```

Use `.u-clear--above` to clear floats above the element to which this class is applied.

```sass
.u-clear--above { clear: both; }
```

## Mixins

If you're writing CSS for a custom component and want to include the behaviour of `u-clear--inside`, you can use the `clear()` mixin. It's available in the [helpers folder](../../src/helpers).

## Examples

```html
<div class="u-clear--inside">
    <p class="u-f--left">This element is floating.</p>
</div>
```

```html
<p class="u-f--left">This element is floating.</p>
<p class="u-clear--above">This element is clearing the float above.</p>
```

## References

- [MDN: clear](https://developer.mozilla.org/en/docs/Web/CSS/clear)
