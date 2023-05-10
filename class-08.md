# Learn CSS - Flexbox

## Flexbox

- Flexbox is a layout mechanism designed for laying out groups of items in one dimension
- It excels at taking a bunch of items which have different sizes, and returning the best layout for those items
- Instead of setting rigid dimensions for the browser to follow, with flexbox, you can instead provide flexible boundaries to hint how the content could display

## What can you do with a flex layout?

- Flex layouts have the following features:
  - They can display as a row, or a column
  - They respect the writing mode of the document
  - They are single line by default, but can be asked to wrap onto multiple lines
  - Items in the layout can be visually reordered, away from their order in the DOM
  - Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent
  - Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties.
  - The items themselves can be aligned on the cross axis

## The main axis and the cross axis

- The main axis is the one set by your flex-direction property
- If that is row your main axis is along the row, if it is column your main axis is along the column
- Flex items move as a group on the main axis
- The corss axis runs in the other direction to the main axis, so if flex-direction is the row the cross axis runs along the column
- you can do two things on the corss axis:
  - you can move the items individually or as a group, so they align against each other and the flex container
  - if you have wrapped flex lines, you can traet those lines as a group to control how space is assigned to those lines

## Creating a flex container

- To use a felxbox you need to declare that you want to use a flex formating context and not regualr block and inline layout, do this by chaning the value of the display property to flex
- The initial value means that:
  - Items display as a row
  - The do not warp
  - They do not wrap
  - They do not grow to full the container
  - They line up at the start of the container

## Controlling the direction of items

- To change the direction, add the property and one of the four values:
  - row: the items lay out as a row
  - row-reverse: the items lay out as a row from the end of the flex container
  - column: the items lay out as a column
  - column-reverse : the items lay out as a column from the end of the flex container

## Reversing the flow of items and accessibilty

- You should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility
- The reordering only happens for the visual order, not the logical order
- Anything which can change the other of items in flexbox or grid can cause this problem

## Writing modes and direction

- flex items lay out as row by default
- a row runs in the direction that senteces flow in your writing mode and script direction
- flex items behave by default is linked to the writing mode of the document
- each axis has a start and an end
- the start of the main axis is referred to as the main-start
- the end of that axis is main-end
- the start of the axis is cross start and the end cross-end start

## Wrapping flex items

- the initial value of the flex-wrap property is nowrap
- this means that if there is not enough space in the container the items will overflow
- Items displaying using the inline values will shrink as small as they can, down to the min-content size before overlfow happpens
- when a flex container warps it creates mulitple flex lines
- each line acts like a new flex container

## The flex-flow shorthand

- you can set the flex-direction and flex wrap properties using the shorthand flex-flow

## Controlling space inside flex items

- assuming our container has more space than is needed to display the items, the items line up at the start and do notw grow to full space
- they stop growing at their max content size
- this is because the intial value of the flex- properties is:
  - flex-grow: 0 - items do not grow
  - flex-shrink 1 - items can shrink small than their flex-basis
  - flex-basis: auto - items have a base size of auto

- This can be represent by a keyword value of flex: intial
- the flex shorthand property, or the longhands of flex-grow, flex-shrink and flex-basis are applied to the children of the flex container
- To cause the items to grow, while allowing large items to have more space than small ones use flex:auto
- This sets the properties to:
  - flex-grow: 1: items can grow larger than their flex-basis
  - flex-shrink: 1: items can shrink smaller than their flex-basis
  - flex-basis: auto: items have a base size of auto

- using flex auto will mean that items end up different sizes, as the space that is shared between the items is shared out after each lis is laid out as max-content size
- this unpacks to:
  - flex-grow: 1: items can grow larger than their flex-basis.
  - flex-shrink: 1: items can shrink smaller than their flex-basis.
  - flex-basis: 0: items have a base size of 0

- using flex: 1 says that all items have a zero size, therefore all of the space in the flex container is available to be distributed
- As all items have a flex-grow factor of 1 they all grow equally and the space is shared equally

## Reordering Flex Items

- Items in your flex container can be reorderd using the order property
- this property allows the ordering of items in ordinal groups
- items are laid out in the firection dictated by the flex-direction, lowest values first
- if more that one items has the same value it will be displayed eith the other items with that value

## Flexbox aliggment overview

- flexbox brought with it a set of poreperties for aligning items and distributing space between items
- the set of poperties can be place into two groups:
  - properties for space distribution
  - properties for alignment
- The poperties that distirbute space are:
  - justify-content: space distribution on the main axis
  - align-content: space distribution on the cross axis
  - place-content: a shorthand for setting both of the above properties

- The propeties used for aligment in flexbox:
  - align-self: aligns a single item on the cross axis
  - align-items: aligns all of the items as a group on the cross axis

## Distributing space on the main axis

- The items lines up at the start of the flex container becuase the initial value of justify-content is flex-start
- The items line up at the start and any extra space is at the end
- you can also distribute space between the items with justify-content: space-between

## With flex-direction: column

- if you have changed your flex-direction to column that justify-content will work on the column
- to have spare space in your container when working as a column you need to give you container a height or block-size

## Distributing space between flex lines

- With a wrapped flex container you might have space to distribute on the cross axis
- In this case you can use the align-content property with the same values as justify-content
- Unlike justify-content which aligns items to flex-start by default, the initial value of align-content is stretch

## The place-content shorthand

- To set both justify-content and align-content you can use place-content with one or two values
-  A single value will be used for both axes, if you specify both the first is used for align-content and the second for justify-content

## Questions

- Flexbox is designed for one-dimensional content. Explain what this means.

It takes a bunch of items with different sizes and returns the best layout for those items

- Explain the difference between the main axis and cross axis.

main-axis is along the row and cross-axis is along the column

- How can using certain properties of flexbox negatively impact accessibility?

Some properties can change the order of the content making it harder to read for some users, cause confusion to screen readers, mess up navigaton on the webpage, and it will also affect any user that rely on assistive technology

- What are some advantages of using flexbox over float?

With flexbox, you have more control over the layout and it also requires less code

- How does this topic connect with your long term goals?

The topic will definitely help me with styling my the content on my page. Just even being able to adjust how content displayed was super hard in the beginning but it looks loke felxbox will make it easier.