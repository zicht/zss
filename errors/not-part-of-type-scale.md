# Not part of type scale

#### Why this error occurred

There are several variables whose value must be present in `$zss--type-scale`. The error
occurs because one of those variables is configured with a value that is not part of the type scale.

#### Possible ways to fix it

The error message contains the name of the violating variable, so find the variable and either:

- change the value of that variable to a value that's present in `$zss--type-scale`.
- add the value to `$zss--type-scale`. Be aware that this will change the values of 
generated `font-size` classes, which will affect the rendering of your design.
