# Borders not in palette

#### Why this error occurred

The variable `$zss--border-colors` contains names or values values that are not defined in `$zss--colors`.

It's only a warning, so the Sass will still compile.

#### Possible ways to fix it

Find the violating names or values in `$zss--border-colors` by comparing them to `$zss--colors` and either:

- change the violating name or value value in `$zss--border-colors` to something that is also defined in `$zss--colors`
- add the violating name or value to `$zss--colors`.
