# Not part of spacing scale

#### Why this error occurred

There are several variables whose value must be present in `$zss--spacing-scale`. The error
occurs because one of those variables is configured with a value that is not part of the spacing scale.

#### Possible ways to fix it

The error message contains the name of the violating variable, so find the variable and either:

- change the value of that variable to a value that's present in `$zss--spacing-scale`.
- add the value to `$zss--spacing-scale`. Be aware that this will change the values of classes
that are generated with the spacing scale, e.g. margins and paddings, which will affect
the rendering of your design.
