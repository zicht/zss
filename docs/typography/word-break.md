# Word Break

ZSS contains utility classes for setting values for the `word-break` property.

## Source files

- [utilities/_word-break.scss](../../src/utilities/_word-break.scss)

## Variables

Since the word break CSS properties have a fixed set of values, there is no variable to configure.   

## Generated CSS

Below is an example of the word break classes that are generated.


```css
.u-break--word { word-break: break-word; }
.u-break--all { word-break: break-all; }
```

## Examples

```html
<div class="u-break--word">This-is-a-very-long-text-line-please-break-it-so-it-doesnt-mess-up-my-layout</div>
```

## References

- [MDN: word-break](https://developer.mozilla.org/en/docs/Web/CSS/word-break)
