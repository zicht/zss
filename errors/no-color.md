# No color

#### Why this error occurred

The mixin `get-color` is called with a color name that is not defined in `$zss--colors`.

#### Possible ways to fix it

The error message contains the name of the invalid color. Check the definition of `$zss--colors` and either:

- find the invalid call in your Sass source code and change the parameter of `get-color` to a value that
_is_ defined in `$zss--colors`.
- add the missing name as a key/value pair to the `$zss--colors` map, e.g. `orange: #f90`.
