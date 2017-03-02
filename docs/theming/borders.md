# Borders

ZSS contains utility classes for setting CSS border properties.

## Source files

- [utilities/_border-color.scss](../../src/utilities/_border-color.scss)
- [utilities/_border-radius.scss](../../src/utilities/_border-radius.scss)
- [utilities/_border-style.scss](../../src/utilities/_border-style.scss)
- [utilities/_border-width.scss](../../src/utilities/_border-width.scss)

## Variables

```sass
$zss--border-colors: $zss--colors !default;
```

`$zss--border-colors` uses the same construct as the [color utilities](colors.md). It is a Sass map where:

- The key is used in the generated class name. 
- The value can be any color format that's understood by CSS (hexadecimal, RGB, HSL et cetera).

```sass
$zss--border-radius-scale: 0 0.125rem 0.25rem 0.5rem !default;
$zss--border-width-scale: 0 0.125rem 0.25rem 0.5rem !default;
```

All border classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

### `border-color`

For each color in `$zss--border-colors` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```sass
.u-bc--black { border-color: #000 }

@media (min-width: 550px) {
    .u-bc--black\@sm { border-color: #000 }
}
```

### `border-radius`

For each numeric value in `$zss--border-radius-scale` and each breakpoint in `$zss--breakpoints`, these classes 
are generated:

```sass
.u-br--0 { border-radius: 0 }
.u-br--t0 { border-top-left-radius: 0 }
.u-br--r0 { border-top-right-radius: 0 }
.u-br--b0 { border-bottom-right-radius: 0 }
.u-br--l0 { border-bottom-left-radius: 0 }

@media (min-width: 550px) {
    .u-br--0\@sm { border-radius: 0 }
    .u-br--t0\@sm { border-top-left-radius: 0 }
    .u-br--r0\@sm { border-top-right-radius: 0 }
    .u-br--b0\@sm { border-bottom-right-radius: 0 }
    .u-br--l0\@sm { border-bottom-left-radius: 0 }
}
```

You can also use border radius to create circles:

```sass
.u-circle { border-radius: 100% }

@media (min-width: 550px) {
    .u-circle\@sm { border-radius: 100% }
}
```

### `border-style`

For each breakpoint in `$zss--breakpoints`, these classes are generated:

```sass
.u-bs--dashed { border-style: dashed; }
.u-bs--t-dashed { border-top-style: dashed; }
.u-bs--r-dashed { border-right-style: dashed; }
.u-bs--b-dashed { border-bottom-style: dashed; }
.u-bs--l-dashed { border-left-style: dashed; }

.u-bs--dotted { border-style: dotted; }
.u-bs--t-dotted { border-top-style: dotted; }
.u-bs--r-dotted { border-right-style: dotted; }
.u-bs--b-dotted { border-bottom-style: dotted; }
.u-bs--l-dotted { border-left-style: dotted; }

.u-bs--solid { border-style: solid; }
.u-bs--t-solid { border-top-style: solid; }
.u-bs--r-solid { border-right-style: solid; }
.u-bs--b-solid { border-bottom-style: solid; }
.u-bs--l-solid { border-left-style: solid; }

@media (min-width: 550px) {
    .u-bs--dashed\@sm { border-style: dashed; }
    .u-bs--t-dashed\@sm { border-top-style: dashed; }
    .u-bs--r-dashed\@sm { border-right-style: dashed; }
    .u-bs--b-dashed\@sm { border-bottom-style: dashed; }
    .u-bs--l-dashed\@sm { border-left-style: dashed; }
    
    .u-bs--dotted\@sm { border-style: dotted; }
    .u-bs--t-dotted\@sm { border-top-style: dotted; }
    .u-bs--r-dotted\@sm { border-right-style: dotted; }
    .u-bs--b-dotted\@sm { border-bottom-style: dotted; }
    .u-bs--l-dotted\@sm { border-left-style: dotted; }
    
    .u-bs--solid\@sm { border-style: solid; }
    .u-bs--t-solid\@sm { border-top-style: solid; }
    .u-bs--r-solid\@sm { border-right-style: solid; }
    .u-bs--b-solid\@sm { border-bottom-style: solid; }
    .u-bs--l-solid\@sm { border-left-style: solid; }
}
```

### `border-width`

For each numeric value in `$zss--border-width-scale` and each breakpoint in `$zss--breakpoints`, these classes 
are generated:

```sass
.u-bw--0 { border-width: 0 }
.u-bw--t0 { border-top-width: 0 }
.u-bw--r0 { border-right-width: 0 }
.u-bw--b0 { border-bottom-width: 0 }
.u-bw--l0 { border-left-width: 0 }

@media (min-width: 550px) {
   .u-bw--0\@sm { border-width: 0 }
   .u-bw--t0\@sm { border-top-width: 0 }
   .u-bw--r0\@sm { border-right-width: 0 }
   .u-bw--b0\@sm { border-bottom-width: 0 }
   .u-bw--l0\@sm { border-left-width: 0 } 
}
```

## Examples

```html
<img class="u-circle" src="image.webp" alt="An image that’s displayed as a circle">

<p class="u-bc--black  u-bw--t1  u-bs--t-solid">Text with a black border at the top.</p>
```

## References

- [MDN: border-color](https://developer.mozilla.org/en/docs/Web/CSS/border-color)
- [MDN: border-radius](https://developer.mozilla.org/en/docs/Web/CSS/border-radius)
- [MDN: border-style](https://developer.mozilla.org/en/docs/Web/CSS/border-style)
- [MDN: border-width](https://developer.mozilla.org/en/docs/Web/CSS/border-width)
