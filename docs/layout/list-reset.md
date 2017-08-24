# List reset object

The list reset object removes margin, padding and bullet styling of ordered and unordered lists.

## Source files

- [objects/_list-reset.scss](../../src/objects/_list-reset.scss)

## Usage

- Add `o-list-reset` to an `<ul>` or `<ol>` element.
    - Optionally, add the modifier `o-list-reset--inline` if the items in the list should
    be aligned horizontally instead of vertically.
- Add `o-list-reset` to child `<li>` elements.


```html
<!-- An inline list -->
<ul class="o-list-reset  o-list-reset--inline">
    <li class="o-list-reset__item">Hodor?</li>
    <li class="o-list-reset__item">HODOR</li>
    <li class="o-list-reset__item">Hodor ...</li>
</ul>
```