# Standards for HTML & SCSS

### Where to apply (S)CSS properties

Properties must be applied to the highest possible ancestor.

In the case that a property can be applied to either one of two siblings, it must be applied to the left-most ot top-most sibling.

### Spacing

Paddings should be used instead of margins to create spacing, except in 3 special cases:

* When a border is used on the element,
* When a negative margin is required,
* To center or push to the right.

### Layout

To build a grid/column layout, `flex` should be used. `float`s must not be used.

To achieve vertical alignment, `flex` should be used.

To achieve horizontal alignment, `flex` should only be used if using `margin: auto` and `text-align: center` cannot be used.
