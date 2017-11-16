# No breakpoint

#### Why this error occurred

One of the responsive mixins is called with a breakpoint name that's not defined. 
The possible mixins are `media-until`, `media-between`, and `media-from`.

#### Possible ways to fix it

The error message contains the name of the invalid breakpoint. Either:

- find the invalid call in your Sass code and change the parameter of the mixin to a correct value.
The correct value is either defined in `$zss--breakpoints`, or in the Sass map that can be passed as
a second parameter to the mixin.
- add the missing name as a key/value pair to the `$zss--breakpoints` map, e.g. `orange: #f90`.
