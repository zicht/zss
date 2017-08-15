# Overflow

ZSS contains utility classes for setting values for the `overflow` property.

## Source files

- [utilities/_overflow.scss](../../src/utilities/_overflow.scss)

## Variables

Since `overflow` has a fixed set of values, there is no variable to configure.   

The overflow classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the generated overflow classes.

```sass
.u-of--auto { overflow: auto; }
.u-of--hidden { overflow: hidden; }
.u-of--scroll { overflow: scroll; }
.u-of--visible { overflow: visible; }
.u-ofx--auto { overflow-x: auto; }
.u-ofx--hidden { overflow-x: hidden; }
.u-ofx--scroll { overflow-x: scroll; }
.u-ofx--visible { overflow-x: visible; }
.u-ofy--auto { overflow-y: auto; }
.u-ofy--hidden { overflow-y: hidden; }
.u-ofy--scroll { overflow-y: scroll; }
.u-ofy--visible { overflow-y: visible; }

@media (min-width: 550px) {
    .u-of--auto\@sm { overflow: auto; }
    .u-of--hidden\@sm { overflow: hidden; }
    .u-of--scroll\@sm { overflow: scroll; }
    .u-of--visible\@sm { overflow: visible; }
    .u-ofx--auto\@sm { overflow-x: auto; }
    .u-ofx--hidden\@sm { overflow-x: hidden; }
    .u-ofx--scroll\@sm { overflow-x: scroll; }
    .u-ofx--visible\@sm { overflow-x: visible; }
    .u-ofy--auto\@sm { overflow-y: auto; }
    .u-ofy--hidden\@sm { overflow-y: hidden; }
    .u-ofy--scroll\@sm { overflow-y: scroll; }
    .u-ofy--visible\@sm { overflow-y: visible; }
}
```

## Examples

```html
<div class="u-of-hidden">
    <p>The parent element prevents this element from overflowing.</p>
</div>
```

## References

- [MDN: overflow](https://developer.mozilla.org/en/docs/Web/CSS/overflow)
