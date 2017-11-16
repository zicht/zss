# Not part of line height scale

#### Why this error occurred

There are several variables whose value must be present in `$zss--line-height-scale`. The error
occurs because one of those variables is configured with a value that is not part of the line height scale.

#### Possible ways to fix it

The error message contains the name of the violating variable, so find the variable and either:

- change the value of that variable to a value that's present in `$zss--line-height-scale`.
- add the value to `$zss--line-height-scale`. Be aware that this will change the values of 
generated `line-height` classes, which will affect the rendering of your design.
