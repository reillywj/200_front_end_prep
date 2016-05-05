# Chapter 1
***
## Building Your First Web Page


### HTML and CSS
**HTML**: HyperText Markup Language

**CSS**: Cascading Style Sheets

### Common HTML Terms

- Elements: `<a> <div> <span> <strong> <em> <h1> ... etc. `
  - an element is the "a", "div", "span" portion of the tag
  - Designate structure of the markup
- Tags
  - "opening tag" marks the beginning of an element `<p>`
  - "closing tag" marks the ending of an element `</p>`
  - The content that falls between the opening and closing tags is the content of that element
- Attributes
  - properties used to provide additional information about an element
  - examples:
    * id: identifies a specific element
    * class: classifies an element
    * src: specifies a source for embeddable content
    * href: provides a hyperlink reference to a linked source

```HTML
<a href="http://shayhowe.com">Shay Howe</a>
```

### Setting Up the HTML Document Structure

- HTML documents are plain text documents saved with an .html file extension rather than a .txt

```
# Required Structure
<!DOCTYPE html>
<html>
  <head>
  </head>

  <body>
  </body>
</html>
```
##### Self Closing Elements:

```HTML
<br>
<embed>
<hr>
<img>
<input>
<link>
<meta>
<param>
<source>
<wbr>
```

- Code validation <a href="http://validator.w3.org/">here</a>

***

### Common CSS Terms

- Selectors
  - designates exactly which element or elements within our HTML to target and apply styles to
  - generally target an attribute value, like id (#id_name) or class (.class_name), or just the element(s)
- Properties
  - determines the styles that will be applied to that element, such as color, font-size, height, width, etc.
- Values
  - setting the property to some style value, like number of pixels, or color name/hexidecimal

### Working with Selectors

- Type Selectors
  - The following CSS selector will apply the styling to all div elements in the HTML

```CSS
div {
  ...
}
```

applies to...

```HTML
<div>1</div>
<div>2</div>
```

- Class Selectors
  - Selects by class, so all elements of that class type will get the designated styling

```CSS
.awesome {
  ...
}
```

applies to...

```HTML
<div class="awesome">...</div>
<a class="awesome" href="www.awesome.com">...</a>
```

- ID Selectors
  - Target only one unique element with given ID

```CSS
#shayhowe {...}
```

applies to...

```HTML
<div id="shayhowe">...</div>
```

- Additional Selectors
  - Many more advanced selectors exist and are readily available

### Referencing CSS

- Must get our CSS talking to our HTML
  - need to reference our CSS file within our HTML
  - Best to include all of our styles in a signle external style sheet, which is referenced from within the `<head>` element of our HTML
  - Single sheet allows us to use the same styles across an entire website and quickly make changes sitewide
- reference using the `<link rel="stylesheet" href="main.css">` tag

### Using CSS Resets

- Each web browser has its own default styles for different elements
- To ensure cross-browser compatibility, CSS resets have become common-place
- CSS resets
  - take every common HTML elements with a predefined style and provide one unified style for all browsers
  - must be at top of style sheet (ensures these are read first and don't override intended stylings)
  - Eric Meyer's reset is very popular: <a href="http://meyerweb.com/eric/tools/css/reset">Eric Meyer reset</a>
  - <a href="http://necolas.github.io/normalize.css">Normalize.css</a> focuses not on using a hard reset for all common elements, but instead on setting common styles for these elements.
