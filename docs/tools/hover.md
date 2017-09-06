# Hover helper

ZSS provides a mixin `hover` to apply CSS when a user interacts with an element.

This mixin is used by ZSS to generate utility classes for background and text colors. (See [theming/colors](../theming/colors.md).)

## Source files

- [helpers/_hover.scss](../../src/helpers/_hover.scss)

## Mixins

### `hover`  

Generates :hover, :active and :focus selectors for an element.
It also provides a `.has-hover-propagation` class to change
elements when the user interacts with a parent element. (See examples below.)

#### Parameters

- `$element`   
   A optional selector that restricts the propagation of the hover effect to 
   the parent element to a certain type of HTML element.

## Examples

```sass
.change-bg {
    @include hover {
        background-color: get-color(red);
    }
}
```

```html
<article class="u-bg--black  has-hover-propagation">
    <h3>Title</h3>
    <p class="change-bg">
        When the parent `article` element is hovered, the background
        color of this text will become red.
    </p>
</article>
```
