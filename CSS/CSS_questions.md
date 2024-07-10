# 1. What is Box model

Every element has a box, the box has width, height, border, padding and margin. One layer surrounds one layer.

Margin -> Border -> Padding -> content box ( defined by height and width )

Padding: Space between border and content.

Border: Space surrounding the padding.

Margin: Space surrounding the border.

# 2. What is the difference in box-sizing between border-box and content-box?

Content-box is the default value of box-sizing. The height and width property only decides the value of content, without border and padding.

Border-box property will make the height and width property including the border and padding. That will make box property more controlled.

# 3. What is flex

Flex means flexible box. It makes layout more flexible by using flexbox. 

1. Flex-direction: define the item layouts in the container
   1. Row: left - right
   2. Column: top - bottom
   3. Row-reverse: right - left
   4. Column-reverse: bottom - top
2. Flex-wrap: define the item wrap property
   1. Wrap: the flex items will be wrapped.
   2. Nowrap: not wrap ( default value ) 
   3. Wrap-reverse: wrap but reversed the order.
3. Flex-flow: flex-direction + flex-wrap
4. Justify-content: set the flex items justify.
   1. Center: center of container.
   2. Flex-start: start of container. ( default value )
   3. Flex-end: end of container.
   4. Space-around: the items display has space between, before and around the items.
   5. Space-between: the items display has space between the lines.
5. Align-items: align for items.
6. Align-content: align for lines.

# 4. What is grid

The most powerful layout system in CSS. It is a 2-dimensional system, which means it can handle both row and column. Flex box is just a 1-dimensional system. Grid layout is more powerful and flexible.