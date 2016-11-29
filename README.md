# ZSS

ZSS is a Sass framework that helps you design and build UI components in a quick and reliable way.

## What it does

- Provides a simple base for your typography.
- Provides abstractions of common UI patterns, so you can focus on the specific design details.
- Generates immutable and configurable utility classes for functional CSS hipness.
- Provides a flexible and configurable flexbox grid, with an optional fallback for ancient browsers.
- Provides a couple of mixins.

In short: it's great at allowing you to build a design without writing a single line of CSS.

## What it doesn’t do

- No design. If you’re looking for a framework to quickly build a prototype that you can discard later, Bootstrap or a specific prototyping tool is a better choice.

## Install

With npm:

```
npm install zss
```

With bower:

```
bower install zss --save-dev
```

## Principles

ZSS is built on a few principles.

- **Composition over repitition**
  The `class` attribute is perfect for composing your design with multiple classes. It leads to better re-usability of your design and smaller CSS stylesheets.
- **Configurable and optional**
  In ZSS, generated utility classes have configurable values. Need an extra value, or don’t like the default values? Just override a variable in your project. Don’t need the button abstraction class? Just don’t import it.
- **Responsiveness**
  All utility classes have responsive equivalents, so you can use different values on different screens.
- **Limit the cascade**
  The cascade is CSS’ greatest feature and liability in one.
