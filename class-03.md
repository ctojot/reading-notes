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

- Making up a block box in CSS we have the:

  - Content box: the are where your content is displayed
  - Padding box:the padding sits around the content as white space
  - Border box: The border box wraps the content and any padding
  - Margin box: The marigin is the most out layer, warpping the content, padding, and border as the whitespace between this box and other elements

#### The Standard CSS Box Model

- In the standard box model, if you give a box an inline-size and a block-size attributes, this defines the inline-size and block-size of the content box

- In the alternative box model, any width is the width of the visible box on the page

### Margins, Paddings, and Borders

#### Margin

- The margin is an invisible space around your box
- It pushes other elements away from the box

#### Margin Collapsing

- Depending on whether two elements whose margins touch have positive or negative margins, the results will be different:
  - Two positive margins will combine to become one margin
  - Two negative margins will collapse and the smallest alue will be used
  - If one margin is negative, its value will be subtracted from the total

- A number of rules dictate when margins do and do not collapse

#### Borders

- The border is drawn between the margin and the padding of a box
- If using the standard box model, the size of the border is added to the width and height of the content box
- If using the alternative box model then the size of the border makes the content box smaller as it takes up some of that available width and height of the element box
- For styling borders, there are a large number of properties, and each border has a style, width, and color that we might want to manipulate

#### Padding

- The padding sits between the border and the content area and is used to push the content away from the border
- Unlike margins, you cannot have a negative padding

### Using Display: Inline-Block

- Display: inline-block is a special value of display, which provides a middle ground between inline and block
- An element with display: inline-block does a subset of the block things we already know about:
  
  - The width and height properties are respected
  - Padding, margin, and border will cause other elements to be pushed away from the box

- It does not, however, break onto a new line, and will only become larger than its content if you explicitly add width and height properties

# Learn JS

- JavaScript is a programming language that allows you to implement complex functionalities on web pages
- Every time a webpage display timely content updates, interactive maps, animated graphics scorlling video jukeboxes, JavaScript was probably involved

## Arrays

### What is an Array?

- Arrays are generally described as "list-like objects"; they are basically single objects that contain multiple values stored in a list
- Array objects can be stored in variables and dealt with in much the same way as any other type of value, the difference being that we can access each value inside the list individually, and do super useful and efficient things with the list, like loop through it and do the same thing to every value
- If we didn't have arrays, we'd have to store every item in a separate variable, then call the code that does the printing and adding separately for each item

### Creating Arrays

- Arrays consist of square brackets and items that are separated by commas

### Finding the Length of an Array

- You can find out the length of an array in exactly the same way as you find out the length of a string by using the length property

### Accessing and Modifying Array Items

- Items in an array are numbered, starting from zero
- This number is called the item's index

### Finding the Index of Items in an Array

- The indexOf() method takes an item as an argument and will either return the item's index or -1 if the item is not in the array

### Adding Items

- To add one or more items to the end of an array we can use push()
- To add an item to the start of the array, use unshift()

### Removing Items

- To remove the last item from the array, use pop()
- To remove the first item from an array, use shift()
- If you know the index of an item, you can remove it from the array using splice()
- In this call to splice(), the first argument says where to start removing items, and the second argument says how many items should be removed

### Accessing Every Item

- You can access every item in an array by using the for... of statment
- You can use map(), to do the same thing to each item in an array leaving you with an array of changed items
- Using filter(), you can create a new array containing only the items in the original array that match some test

### Converting bewteen Strings and Arrays

- Often you'll be presented with some raw data contained in a big long string, and you might want to separate the useful items out into a more useful form and then do things to them, like display them in a data table
- To do this, we can use the split() method

### Active Learning: Top 5 Searches

- A good use for array methods like push() and pop() is when you are maintaining a record of currently active items in a web app
- The idea is that when terms are entered in the search box, the top 5 previous search terms are displayed in the list
- When the number of terms goes over 5, the last term starts being deleted each time a new term is added to the top, so the 5 previous terms are always displayed

## Expressions and Operators

- An expression is a valid unit of code that resolves to a value
- Two types of expressions:
  
  - those that have side effects
  - those that purely evaluate

- JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator
- A binary operator requires two operands, one before the operator and one after the operator

- operators:
  - Assignment
  - Comparison
  - Arithmetic
  - Bitwise
  - Logical
  - BigInt
  - String
  - Conditional (terneary)
  - Comma
  - Unary
  - Relational

- These operators join operands either formed by higher-precedence operators or one of the basic expressions
- JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator

### Assignment Operators



## Questions

- When should you use an unordered list in your HTML document?

You should use an unordered list when you have a list of items that can don't need to be presented in a certain order

- How do you change the bullet style of unordered list items?

You can change the bullet style of an unordered list using the type attributre

- When should you use an ordered list vs an unorder list in your HTML document?

The only time you need to use an ordered list is when the items need to be presented in a meaningful order

- Describe two ways you can change the numbers on list items provided by an ordered list?

You can use the reverse attirubte to number them in reverse or you can use the type attribute to set the number typing

- Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?


- List and describe the four parts of an HTML elements box as referred to by the box model.

padding

margin

border

width

- What data types can you store inside of an Array?

Arrays consist of single objects with multiplpe values

- Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

The people array is a valid JavaScript array becuase of the multiple values that the person has.

- List five shorthand operators for assignment in javascript and describe what they do.

x = f() : Assignment

x += f() : Addition

x -= f() : Subtraction

x *= f() : Mulitiplication

x /= f() : Division

- Read the code below and evaluate the last expression and explain what the result would be and why.

The result would be 10dog because false as a number would be 0 so we can the equation is (10 + 0) + 'dog'. 

- Describe a real world example of when a conditional statement should be used in a JavaScript program.

An real world example would be when a mother tell her child if they help her with a chore, they'll get rewarded with extra allowance

- Give an example of when a Loop is useful in JavaScript.

Loops are useful when we have to do a certain task multiple times. An example would be drawing a circle 100 times. We could code a loop that creates the circle 100 times and it would be much faster than righting a code to make one circle a 100 times