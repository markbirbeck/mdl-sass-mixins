# mdl-sass-mixins

Sass Rules using the CSS from Material Design Lite (MDL) as mixins.

For the motivation for this module as well as information about how to use it, see the blog post [A Mixin Approach to Material Design Lite Using Sass][mixin post].

[mixin post]: <http://bit.ly/1LPY2GT>

## Adding the MDL Styles

To make the styles from MDL available to this project we import MDL's `material.css` file into our own stylesheet.

To get a copy of `material.css` it's actually better to grab the whole MDL project from NPM, which is why we've added `material-design-lite` as a Node module.

By having a clear dependency on MDL (rather than manually importing a single file from the module) we can do things like pin our own stylesheet to a particular version of MDL.

To make use of the styles we simply use an `@import` statement to include the stylesheet into our own stylesheet:

```css
@import "node_modules/material-design-lite/material";
```
