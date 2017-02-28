# Backgrounds

ZSS contains utility classes for setting CSS properties concerning background images.

## Referenced files

- [utilities/_background-size.scss](../../src/utilities/_background-size.scss)

## Variables

Since the background CSS properties have a fixed set of values, there is no variable to configure.   

The background classes come with responsive equivalents. The exact breakpoints are defined in `$zss--breakpoints`.

## Generated CSS classes

Below is an example of the background classes that are generated.

`background-size`:

```
.u-bg--contain { background-size: contain; }
.u-bg--cover { background-size: cover; }

@media (min-width: 550px) {
    .u-bg--contain\@sm { background-size: contain }
    .u-bg--cover\@sm { background-size: cover }
}
```
