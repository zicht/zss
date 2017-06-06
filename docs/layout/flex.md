# Flex

ZSS contains utility classes for setting flexbox related CSS properties.

## Source files

- [utilities/_flex.scss](../../src/utilities/_flex.scss)

## Variables

Since the flexbox properties have a fixed set of values, there is no variable to configure.   

The flex classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the classes that are generated.

```sass
.u-flex--auto { flex: 1 1 auto; }
.u-no-flex { flex: none; }

.u-flex--column { flex-direction: column; }
.u-flex--row { flex-direction: row; }

.u-flex--items--start { align-items: flex-start; }
.u-flex--items--end { align-items: flex-end; }
.u-flex--items--center { align-items: center; }
.u-flex--items--base { align-items: baseline; }
.u-flex--items--stretch { align-items: stretch; }

.u-flex--content--start { align-content: flex-start; }
.u-flex--content--end { align-content: flex-end; }
.u-flex--content--center { align-content: center; }
.u-flex--content--base { align-content: baseline; }
.u-flex--content--stretch { align-content: stretch; }

.u-flex--self--start { align-self: flex-start; }
.u-flex--self--end { align-self: flex-end; }
.u-flex--self--center { align-self: center; }
.u-flex--self--base { align-self: baseline; }
.u-flex--self--stretch { align-self: stretch; }

.u-flex--justify--start { justify-content: flex-start; }
.u-flex--justify--end { justify-content: flex-end; }
.u-flex--justify--center { justify-content: center; }
.u-flex--justify--base { justify-content: baseline; }
.u-flex--justify--stretch { justify-content: stretch; }

.u-order--first { order: -1; }
.u-order--1 { order: 1; }
.u-order--2 { order: 2; }
.u-order--3 { order: 3; }
.u-order--4 { order: 4; }
.u-order--last { order: 666; }

@media (min-width: 550px) {
    .u-flex--auto\@sm { flex: 1 1 auto; }
    .u-no-flex\@sm { flex: none; }

    .u-flex--column\@sm { flex-direction: column; }
    .u-flex--row\@sm { flex-direction: row; }

    .u-flex--items--start\@sm { align-items: flex-start; }
    .u-flex--items--end\@sm { align-items: flex-end; }
    .u-flex--items--center\@sm { align-items: center; }
    .u-flex--items--base\@sm { align-items: baseline; }
    .u-flex--items--stretch\@sm { align-items: stretch; }

    .u-flex--content--start\@sm { align-content: flex-start; }
    .u-flex--content--end\@sm { align-content: flex-end; }
    .u-flex--content--center\@sm { align-content: center; }
    .u-flex--content--base\@sm { align-content: baseline; }
    .u-flex--content--stretch\@sm { align-content: stretch; }

    .u-flex--self--start\@sm { align-self: flex-start; }
    .u-flex--self--end\@sm { align-self: flex-end; }
    .u-flex--self--center\@sm { align-self: center; }
    .u-flex--self--base\@sm { align-self: baseline; }
    .u-flex--self--stretch\@sm { align-self: stretch; }

    .u-flex--justify--start\@sm { justify-content: flex-start; }
    .u-flex--justify--end\@sm { justify-content: flex-end; }
    .u-flex--justify--center\@sm { justify-content: center; }
    .u-flex--justify--base\@sm { justify-content: baseline; }
    .u-flex--justify--stretch\@sm { justify-content: stretch; }

    .u-order--first\@sm { order: -1; }
    .u-order--1\@sm { order: 1; }
    .u-order--2\@sm { order: 2; }
    .u-order--3\@sm { order: 3; }
    .u-order--4\@sm { order: 4; }
    .u-order--last\@sm { order: 666; }
}
```

## Examples

```html
<div class="u-flex  u-flex--justify--end  u-flex--items--end">
    <p>This element is aligned to the bottom right of the box</p>
</div>
```

```html
<div class="u-flex">
    <p>This element is shown first on mobile screens</div>
    <p class="u-order--first@lg">This element is shown first on bigger screens</p> 
</div>
```

## References

- [MDN: align-content](https://developer.mozilla.org/en/docs/Web/CSS/align-content)
- [MDN: align-items](https://developer.mozilla.org/en/docs/Web/CSS/align-items)
- [MDN: align-self](https://developer.mozilla.org/en/docs/Web/CSS/align-self)
- [MDN: flex](https://developer.mozilla.org/en/docs/Web/CSS/flex)
- [MDN: flex-direction](https://developer.mozilla.org/en/docs/Web/CSS/flex-direction)
- [MDN: justify-content](https://developer.mozilla.org/en/docs/Web/CSS/justify-content)
- [MDN: order](https://developer.mozilla.org/en/docs/Web/CSS/order)
