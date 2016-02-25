#Front End Prep
####25 Feb 2016


##Getting Started with HTML
#####Elements
- `<html></html>`
- DTD for doctype: <!doctype html>
- `<body></body>` element
  - Container representing the entire page body
  - All content is to be rendered to the screen nested within it
- `<head></head>` element
  - Useful to browser when constructing the page, but is not actually part of the content of the page
- META ELEMENT:
  - `<meta ... />`
  - contains any data about our page that may be nice for the browser to have, but isn't necessary for displaying
  - a "self-closing" element
- Browser does not display pre-formatted text on its own. It relies on the elements to let it know how and where to change formatting.

- paragraph element: `<p></p>`
  - wrap a single paragraph of text to let the browser know to have it on its own row
  - spacing added above and below the paragraph
- Heading element: `<h1></h1>`
  - In HTML, page content thought of as a chapter or book online
  - heading 1 means our heading is the most important heading on the page
  - subheadings with subsequent numbers down to `<h6>`

- Other elements:
  - strong: bold, with stronger importance
  - em: italicized, part of sentence to receive emphasis
  - b: bold
  - i: italicized, no change in meaning
  - sub: subscript
  - sup: superscript
  -div and span
    - containers that don't add any sort of additional meaning to the content
    - don't apply any additional semantic meaning to its content
    - div
      * block elements by default
    - span
      * inline by default

####Attributes
- Variable names of the HTML world
- Additional pieces of info meant for the browser
- Tell the browser to do something specific with the value given to the attribute
- Written with "name" and "value"

```HTML
<meta charset="utf-8" />
```

---
##Styling with CSS

- CSS: Cascading Style Sheets
  - Instructions for the browser on how to present everything visually
  - Think: spacing, colors, font styles, and even background images

**Property**
- property + value pairs:
- tells browser which aspect of the element's design to change with the supplied value

E.g.

```CSS
color: red;
```

**Style Attribute**

- A few HTML attributes are universally available, meaning they can be added to any HTML element

```HTML
<h1 style="color: orange;">Hello Internet</h1>
```

- color and font-size
  - inheritance property: text inside this container also receive its changes

**Text-align**

- Styling inside the HTML element can be cumbersome and not DRY


###Style Element in HTML

```HTML
<style type="text/css"></style>
```

- This tells the browser to take the contents of the style element and assume it's CSS


###CSS Selectors

- Tells browser what style instructions are to be applied to which elements
- Special notation for targeting one or more HTML elements by either the element name or some attribute on the alement

####Element selector

```HTML
h1 {
  color: orange;
  text-align: center;
}
```

####ID and Class Selectors

- two most common methods: class and ID
  - ID must be unique to all of the ID values
  - Any number of elements can have the same class name
  - class can also contain multiple names
  - #id_name to select id
  - .class_name to select class

```HTML
<p id="id_name">

#id_name {
  font-size: 18px;
}

.highlight {
  background-color: #f0f099;
}
```

### Hex Colors















