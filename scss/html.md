# Tenatek standards for HTML & SCSS

* Properties must be applied to the highest possible ancestor
* In case a property can be applied to either one of two siblings, it must be applied to the left-most ot top-most sibling
* Paddings should be used instead of margins, except in 3 special cases:
  * When a border is used on the element,
  * When a negative margin is required,
  * To center or push to the right.
