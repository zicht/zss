# Transition

Contains options for a smooth animation of transitions between element states.

## Source files

- [utilities/_transition.scss](../../src/utilities/_transition.scss)

## Variables
Since the transitions have a fixed set of values, there are no variables to configure.

## Generated CSS
Below is an example of the transition classes that are generated.
````
.u-trans--all { transition: all 150ms ease-in; }
.u-trans--bc { transition: border-color 150ms ease-in; }
.u-trans--bg { transition: background-color 150ms ease-in; }
.u-trans--color { transition: color 150ms ease-in; }
````

## Usage

- Add `u-trans--color` to an `<a>` or any other element where a color needs to be animated smoothly Requirement is that this element has both a default color, like `u-black` and a hover-class like `u-hover--red`.
Transition options are:

## Examples
````
<a href="#" class="u-black  u-hover--red  u-trans--color">
    My color changes smoothly from black to red on hover
</a>
````

## References
- [MDN: transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)