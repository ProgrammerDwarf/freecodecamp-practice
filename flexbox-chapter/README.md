# A flexible tool

Flexbox is a tool that allows us to make flexible layouts. Thus, We can adapt each part of out page to differents viewports.
Also, We have to notice and remember that this is a one-dimension layout method.

## A relationship of two key elements

First, We need a parent element and second, its children elements.  

- Parent: Element that has one or more children in it.
- Children: Elements that are inside of a container.

### Properties for the parent

- `display: flex`: this is the attribute that we have to assign to a parent element. The entire interior of this container will become a flexible element. This will happen as long as the width of the child elements are not declarated.
Another thing about this property is that when used, the child elements will expand to fill the entire container evenly.
- `flex-direction`: it has two main options: row and column, but there are other possibilities.
  - `row`
  - `column`
  - `reverse row`
  - `column-reverse`
The last two will not change the order of the elements on the HTML side. In fact, this will change the way the elements appear only visually.

- `justify-content`: Each Flex container has to axes in it. The main axes, which is horizontally by default, and the cross axe, perpendicular to the first axe.  
  - `flex-start`: aligns items to the start of the flex container. For a row, this pushes the items to the left of the container. For a column, this pushes the items to the top of the container. This is the default alignment if no justify-content is specified.
  - `flex-end`: aligns items to the end of the flex container. For a row, this pushes the items to the right of the container. For a column, this pushes the items to the bottom of the container.
  - `space-between`: aligns items to the center of the main axis, with extra space placed between the items. The first and last items are   pushed to the very edge of the flex container. For example, in a row the first item is against the left side of the container, the last item is against the right side of the container, then the remaining space is distributed evenly among the other items.
  - `space-around`: similar to space-between but the first and last items are not locked to the edges of the container, the space is distributed around all the items with a half space on either end of the flex container.
  - `space-evenly`: Distributes space evenly between the flex items with a full space at either end of the flex container.

- `align-items`: In the same way We can align items horizontally We could do it with this property along the cross axis.
  - `flex-start`: aligns items to the start of the flex container. For rows, this aligns items to the top of the container. For columns, this aligns items to the left of the container.
  - `flex-end`: aligns items to the end of the flex container. For rows, this aligns items to the bottom of the container. For columns, this aligns items to the right of the container.
  - `center`: align items to the center. For rows, this vertically aligns items (equal space above and below the items). For columns, this horizontally aligns them (equal space to the left and right of the items).
  - `stretch`: stretch the items to fill the flex container. For example, rows items are stretched to fill the flex container top-to-bottom. This is the default value if no align-items value is specified.
  - `baseline`: align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.

  - `wrap`: This will grab all our internal buddies and ordering ,by applying some calculation about its heights and width, in a new line if it is needed. Note that the child elements has to have its heights and widths well declarated.

  -`nowrap`: this is the default setting, and does not wrap items.
  -`wrap`: wraps items from left-to-right if they are in a row, or top-to-bottom if they are in a column.
  -`wrap-reverse`: wraps items from right-to-left if they are in a row, or bottom-to-top if they are in a column.

## Child Items Behavior

  Inside the flexbox world We have to remember that the child are part of this system and they have their own properties.

  -`flex-shrink`: It will assign a coefficient, it could be a positive number and as larger the number is it will shrink more than the other flex child. This will happen as long as the container and the child have no width declarated or the width of the container is less than the width of the child.
  -`flex-grow`: The exact opposite of the shrink property, this will expand the children items inside the container within the relation of the number values on each child.
  -`flex-basis`: Declaration of the initial size of the item within the container.
  -`order`: The order property is used to tell CSS the order of how flex items appear in the flex container. By default, items will appear in the same order they come in the source HTML. The property takes numbers as values, and negative numbers can be used.  
  -`align-self`: The final property for flex items is align-self. This property allows you to adjust each item's alignment individually, instead of setting them all at once. This is useful since other common adjustment techniques using the CSS properties float, clear, and vertical-align do not work on flex items. Align-self accepts the same values as align-items and will override any value set by the align-items property.
  