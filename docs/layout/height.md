# Height

ZSS contains utility classes for setting values for the `height` property.

## Source files

- [utilities/_height.scss](../../src/utilities/_height.scss)

## Variables

```sass
$zss--height--scale: 1rem 2rem 4rem 8rem !default;
$zss--height--percentage-scale: 25 50 75 100 !default;
```

All height classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS

For each value in `$zss--height--scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-height--1 { height: 1rem; }
.u-height--2 { height: 2rem; }
.u-height--3 { height: 4rem; }
.u-height--4 { height: 8rem; }

@media (min-width: 550px) {
    .u-height--1\@sm { height: 1rem; }
    .u-height--2\@sm { height: 2rem; }
    .u-height--3\@sm { height: 4rem; }
    .u-height--4\@sm { height: 8rem; }
}
```

For each value in `$zss--height--percentage-scale` and each breakpoint  in `$zss--breakpoints`, these classes are generated:

```css
.u-height--25 { height: 25%; }
.u-height--50 { height: 50%; }
.u-height--75 { height: 75%; }
.u-height--100 { height: 100%; }

@media (min-width: 550px) {
    .u-height--25\@sm { height: 25%; }
    .u-height--50\@sm { height: 50%; }
    .u-height--75\@sm { height: 75%; }
    .u-height--100\@sm { height: 100%; }
}
```

Furthermore, there are a couple of classes that are not defined in variables.

```css
.u-height--auto { width: auto; }
.u-height--25v { height: 25vh; }
.u-height--50v { height: 50vh; }
.u-height--75v { height: 75vh; }
.u-height--100v { height: 100vh; }

@media (min-width: 550px) {
    .u-height--auto\@sm { width: auto; }

    .u-height--25v\@sm { height: 25vh; }
    .u-height--50v\@sm { height: 50vh; }
    .u-height--75v\@sm { height: 75vh; }
    .u-height--100v\@sm { height: 100vh; }
}
```

## Examples

```html
<section>
    <div class="u-height--50@lg">This element has a height of 50% of its parent on desktop.</div>
</section>
```

## References

- [MDN: height](https://developer.mozilla.org/en/docs/Web/CSS/height)
