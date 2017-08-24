# Vertical alignment

ZSS contains utility classes for setting values for the `vertical-align` property.

## Source files

- [utilities/_vertical-align.scss](../../src/utilities/_vertical-align.scss)

## Variables

Since `vertical-align` has a fixed set of values, there is no variable to configure. 

The classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

Below is an example of the classes that are generated.

```sass
.u-valign--sub { vertical-align: sub; }
.u-valign--super { vertical-align: super; }
.u-valign--text-top { vertical-align: text-top; }
.u-valign--text-bottom { vertical-align: text-bottom; }
.u-valign--middle { vertical-align: middle; }
.u-valign--top { vertical-align: top; }
.u-valign--bottom { vertical-align: bottom; }
.u-valign--baseline { vertical-align: baseline; }

@media (min-width: 550px) {
    .u-valign--sub\@sm { vertical-align: sub; }
    .u-valign--super\@sm { vertical-align: super; }
    .u-valign--text-top\@sm { vertical-align: text-top; }
    .u-valign--text-bottom\@sm { vertical-align: text-bottom; }
    .u-valign--middle\@sm { vertical-align: middle; }
    .u-valign--top\@sm { vertical-align: top; }
    .u-valign--bottom\@sm { vertical-align: bottom; }
    .u-valign--baseline\@sm { vertical-align: baseline; }
}
```

## Examples

```html
<p class="u-inline-block  u-valign--middel">This element has text that's vertically aligned to the middle.</p>
```

## References

- [MDN: vertical-align](https://developer.mozilla.org/en/docs/Web/CSS/vertical-align)
