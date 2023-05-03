# Learn HTML

## HTML: HyperText Markup Language

- HTML is the most basic building block of the web
- "Hypertext" refers to links that connect webpages to one another, either within a single website or multiple websites
- HTML uses markup to annotate text, images, and other content for display in a website

## Ordered Lists

- The ol html element represents an ordered list of items usually as a numbered list

### Attributes

- The element also accpets the global attributes:

  - reversed: lists the items in reverse
  - start: an integer to start counting from
  - type: sets the number typing

### Usage Notes

- Ordered lists are typically displayed with a preceding marker
- The difference between ol and ul is that ol is meaningful

## Unordered Lists

- The ul html element represents unordered lists

### Attributes

- Also accepts global attributes

  - compact: list is rendered in a compact style
  - type: sets the list in bullet style

### Usage Notes

- The ul elements is manly for grouping a collection of items that don't really have a numerical ordering to them

# Learn CSS

## Learn to Style HTML with CSS

- Cascading Style Sheets (CSS) is the first thing you need to learn after learning html
- HTML is used to structure and CSS is used to style

## The Box Model

- Everything is CSS has a box around it and the key to CSS is understanding it to create more complex CSS styling

### Block and Inline Boxes

- In CSS there are several types of boxes that fit into categories of *block boxes* and *inline boxes*

### Outer Display Type

- If a box has an outer display type of box:

  - the box will break onto a new line
  - width and height are respected
  - padding, margin, and border will cause other elements to be pushed away from box

- Some elements like h1 and p use block as their display type by default

- If a box has an outer display type of inline, then;

  - the box will not break onto a new line
  - width and height will not apply
  - top and bottom padding, margin, and borders will apply but will not cause other inline boxes to move away from the box
  - left and right padding, margin, and border will apply and will casue other inline boxes to move away from the box

- a, span, em, and strong use inline as their outer display by default

### Inner Display Type

- Boxes also have an inner display type that determines how elements inside the box are laid out
- Block and inline layout is the default way thing behave on the web

### Examples of Different Display Types

- 3 html elements that have an outer display type of block

  - A paragraph with a border added in CSS
  - A list using display:flex
  - A block-level paragraph with two span elemetns inside

### What is the CSS Box Model?

- The CSS box model applies to block boxes and how the different parts of a box work together to create a box you see on a page

#### Parts of a Box 

- 