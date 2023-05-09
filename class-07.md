# Domain Modeling

- Domain modeling is the process of creating a conceptual model in code for a specific problem
- An object-oriented model an entity that stores data in the properties and encapsulates behaviors in methods
- A domain model that's articulated well can verify and validate the understanding of a specific among various stake holders

## Define A Constructor and Intialize Properties

- Use a cunstructor function to define the same properties between many objects
- Writing and testing code will help you remember how to implement domain models
- Math.random models a random number generator
- Methods can be added to a functions prototype

# HTML Table Basics

## What is a Table?

- A table is a structured set of data made up of rows and columns (tabular data)
- A table allows you to quickly and easily look up values that indicate some kind of connection between different types of data

### How Does a Table Work?

- Information is easily interpreted by making visual associations between row and column headers

### Table Styling

- for tables to be effective on the web, you need to provide some styling information with CSS, as well as good solid structure with HTML

### When You Shoulf NOT Use HTML Tables

- HTML tables are used for tabular data, however some people used to use it to layout webpages because of terrible CSS intergration
- The main reason using tables for layout rather than CSS layout technique is bad because
  - Layout tables reduce accessibilty for visually imparied
  - Tables prduce tag soup
  - Tables are not auto responsive

## Adding Headers with th Element

- Table headers are special cells that go at the start of a row or column and define the data in that row or column

### Why Headers are Useful 

- Its easier to find the data you are looking for
- They also allow you to make tables for accessible

## Allowing Cells to Span Multiple Rows and Columns

- Table headers and cells have the colspan and rowspan attributes that allow us to span accros and span downwards
- Both accept unitless number value

## Providing Common Styling to Columns

### Styling Without col

- HTML has a method of defining styling information for an entire column of data in one place, col and colgroup elements
- You must sepcify styling information on evey td or th in the column or use a complex selector such as :nth-child because its annoying and inefficient to specify styling on clumns

### Styling with col

- col elements are specified inside colgroup container just below the opening table tag
- Just like colspan and rowspan, span takes a unitless number value that specifies the number of columns you want the styling to apply to

# Introducing Constructors

- Using object literals is fine when you only need to create one object, but if you have to create more than one, they're inadequate
- We would like a way to define the "shape" of an object, the set of methods and the properties it can have, and then create as many objects as we like, just updating the values for the properties that are different
- When you call a constructor, it will:
  - create a new object
  - bind this to the new object, so you can refer to this in your constructor code
  - run the code in the constructor
  - return the new object

# Object Prototypes Using A Constructor

- Objects are foundational to almost every aspect of JS
- Objects are key/value paris
- Create objects with {} and add properties and methods to an object using dot notations
- Next step is to encapsulate logic inside of a function that can be envoked when needed

## Functional Instantiation

- Instead of recreating methods, we move them to their own object, then we an have each variable represent that object

## Functional Instantiation with Shared Methods

- By moving the shared methods to their own object and referencing that object inside of our variable function, we've now solved the problem of memory waste and overly large variable objects

## Object Create

- object.create allows you to create an object which will delegate to another object on failed lookups

## Questions

- Explain why we need domain modeling.

It helps you understand and represent the structure and behavior of a specific problem domain

- Why should tables not be used for page layouts?

Tables are now intended for displaying tabular data

- List and describe 3 different semantic HTML elements used in an HTML table.

th
td

- What is a constructor and what are some advantages to using it?

A constructor is a special method that is used to initialize objects when they're created. The advantages are encapsulation, code reuse, and can be used to create object of different types that share common things

- How does the term this differ when used in an object literal versus when used in a constructor?

this refers to the object itself. You use to refer to objects being created by the constructor

- How does the term this differ when used in an object literal versus when used in a constructor?

- Explain prototypes and inheritance via an analogy from your previous work experience.
