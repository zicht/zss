# Configuration

ZSS generates a bunch of CSS classes. You can control what is generated and customize it to your design needs.

- Most utility classes are based on some sort of scale. It has sane defaults you can use to quickly build a prototype, but if you can customize the values if needed.
- There are several component _abstractions_, like buttons and grids. If you don't want to use them, don't import them in your Sass file.

## Customizing

All variables are located in `~/scss/variables/_zss-defaults.scss`. You can override them at will. Re-declare them in a file and import that file into your main Sass file.

```
@import '../bower_components/zss/scss/variables/zss-defaults';
@import 'variables/your-own-file-with-custom-values';
```