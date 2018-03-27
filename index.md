## Tags and attributes

### Tags

The most appropriate tags should always be used. In particular, this means that:

- `button` tags should be used for JavaScript actions whereas `a` tags should be used for navigation,
- `p` tags should be used for texts of more than 80 characters, composed of full sentences,
- `i` tags should be used for icons,
- `span` tags should be used to highlight parts of a text.

### Attributes

#### Attribute uniqueness

Within a tag, a given attribute should only appear once. 

#### Quote usage

Double quotes (`""`) should be used to enclose the attribute's value.

#### Whitespace in attributes

The attribute's value should not contain unnecessary whitespace.

## Structuring the document

### `doctype`

Full HTML documents should begin with the `<!doctype html>` declaration, in lowercase.

### `head`

#### Mandatory elements

The `head` tag's first direct descendants should be:

```html
<title>Website/Page Title</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
```

#### Accepted elements

After the mandatory elements, `link` tags can be added to include CSS stylesheets and other assets. 

#### Forbidden elements

No `script` tags should appear in the `head`.

### Body

#### Accepted direct descendants

The `body` tag's direct descendants should be either of type `nav`, `section`, or `script`. The `script`s should appear last in the `body`.

#### `nav`

Only one of the `body`'s immediate children should be of type `nav`.

## Structuring elements

### Header tags (`h1`, `h2`, etc.)

#### One header tag per element

A given element can only contain one header tag as a direct descendant. 

#### Same header tag at the same level

If two elements at the same level of the DOM tree contain a header tag, then it must be the same.

#### Lower-level header tags at lower levels

If a given header tag has been used at a given level of the DOM tree, then all elements at lower levels of the DOM tree can contain only lower-level header tags.

## Class names

### Standard class names

#### Text

For elements that contain primarily text, such as `p`s, the class name `text` should be used.

#### Title

For elements that wrap titles, the class name `title` should be used.

#### Image

For elements that wrap images, the class name `image` should be used.

#### Wrapper

For generic wrappers, the class name `wrapper` should be used.

#### List items

For list items, usually the immediate children of a `wrapper`, the class name `item` should be used.

### Standard class names and nesting

When an element's descendant has the same class name as the element itself, there is a risk of collision. Therefore, when nesting elements with the same class name, a numeric suffix should be added, as such:

```html
<div class="wrapper-1">
  <div class="item-1">
    <div class="wrapper-2">
      <div class="item-2"></div>
      <div class="item-2"></div>
    </div>
  </div>
  <div class="item-1">
    ...
  </div>
  <div class="item-1">
    ...
  </div>
</div>
```

### Non-standard class names

When the above standard class names do not apply, custom class names need to be defined, taking into account the following:

- Class names should be descriptive of the content of the element they are applied to. Inspiration can be drawn from the element's images, text, or colors,
- Class names should be short and simple. Hyphens should be avoided,
- Class names should not contain abbreviations (e.g. `col` for `column`).
