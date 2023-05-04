# Creating Hyperlinks

- Hyperlinks are what make the web the web

## What is a Hyperlink

- Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address

## Anatomy of a Link

- A basic link is created by wrapping the text or other content inside an a element and using the href attribute, also known as a Hypertext Reference, or target, that contains the web address

### Block Level Links

- Almost any content can be turned into a link, including block-level elements

### Image Links

- Use the a element to wrap the image file referenced with the img element

### Adding Supporting Information with the Title Attribute

- The title contains additional information about the link, such as which kind of information the page contains, or things to be aware of on the website

## A Quick Primer on URLs and Paths

- A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web
- URLs use paths to find files
- Paths tell you where the file is located in the filesystem
- When working locally with a website, you'll have one directory that contains the entire site

### Documend Fragments

- It's possible to link to a specific part of an HTML document, known as a document fragment, rather than just to the top of the document

### Abosolute Versus Relative URLs

- Two terms you'll come across on the Web are absolute URL and relative URL:
- absolute URL: Points to a location defined by its absolute location on the web, including protocol and domain name

## Link Best Practices

### Use Clear Link Wording

- We need to make our links accessible to all readers, regardless of their current context and which tools they prefer
  - Screen reader users like jumping around from link to link on the page, and reading links out of context
  - Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to
  - Visual readers skim over the page rather than reading every word, and their eyes will be drawn to page features that stand out, like links

## Email Links

- it's possible to create links or buttons that, when clicked, open a new outgoing email message rather than linking to a resource or page

### Specifiying Details

- In addition to the email address, you can provide other information
- The most commonly used of these are subject, cc, and body

# CSS Layout: Normal FLow

- You can change how elements behave either by adjusting their position in normal flow or by removing them from it altogether
- It ensures that your content is readable even if the user's using a very limited browser or a device such as a screen reader that reads out the content of the page

## How Are Elements Laid Out by Default?

- The process begins as the boxes of individual elements are laid out in such a way that any padding, border, or margin they happen to have is added to their content is called the box model
- By default, a block level element's content fills the available inline space of the parent element containing it and the element grows along the block dimension to accommodate its content
- The size of inline elements is just the size of their content
- The normal layout flow is the system by which elements are placed inside the browser's viewport
- Inline elements behave differently, they don't appear on new lines; instead, they all sit on the same line along with any adjacent text content as long as there is space for them to do so inside the width of the parent block level element

# CSS Layout: Positioning

- Positioning allows you to take elements out of normal document flow and make them behave differently

## Introducing Positioning

- Positioning allows us to produce interesting results by overriding normal document flow
- There are a number of different types of positioning that you can put into effect on HTML elements

## Static Positioning

## Questions

- To create a basic link, we wrap text or other content inside what element?

a element

- The href attribute contains what information?

href contains the web address

- What are some ways we can ensure links on our pages are accessible to all readers?

By using clear link wording becuase some readers like jumping around and will read links out of context. Some will skim through content and their eyes will be drawn to visiual features like the links

- What is meant by “normal flow”?

Normal is basically the default behavior of webpage elements when you haven't made any changes to the layout

- What are a few differences between block-level and inline elements?

Block-level:

    - take up full width be default
    - begin on a new line and push content to a new line
    - Width, height, margin, and padding can be changed set css

Inline:
    - Only take up necessary width and height of their content
    - Do not start on a new line by default
    - Width, height, margin, and padding can **NOT** be set with CSS

- ___ positioning is the default for every html element.

Static Positioning

- Name a few advantages to using absolute positioning on an element.

Some advantages are you get precise control element postioning. You can use it to overlap elements. It can also be combined with css to create animation and movement as well as custom layouts

- What is a key difference between fixed positioning and absolute positioning?

Fixed positioning
    - remain in the same position even when the page is scrolled through

Absolute positioning
    - positions an element relative to its nearest positioned ancestor
    - absolute positioned elements are removed from the normal flow and do not take up space in the document flow

