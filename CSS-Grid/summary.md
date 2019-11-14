# This is the CSS GRID chapter

Here, we will learn about the 2D design tool that is CSS-GRID:

## The idea of working in 2D

In addition to Flexbox, the Grid has the facility to work (simultaneously) horizontally and vertically. Flexbox has its way
To refer to its internal elements, Grids also has it. Here, we divide the page into rows and columns. The first works
horizontally and the last works vertically.

## A parents relationship

First, We need two key characters here: the parent and the child element.

## First property here

- `grid`: By setting the `display: grid` on the parent will not cause any changes (visually I mean) on the page but I'll tell to the browser
that it will be the container.

## What's next`?`

Well, now I will list the properties to use the grid:

- `grid-template-columns`: This will be the amount of columns that We'll have and how much is their width.
Example: `grid-temple-row: 1fr 20px 50%`. Here there will be three columns each with a different width. We know the last two, but the first one referred to a fraction of the free space that the container has.

- `grid-template-row`: The same behavior of the columns but this time we are controlling the height of the rows.

- `grid-column-gap`: Controls the length between the columns.

- `grid-row-gap`: Controls the length between the columns.

- `grid-gap`: this is the shorthand for setting the last two properties. Being the first grid-row-gap and the second grid-column-gap.

- `grid-column`: Imagine a grid like this:  

| box1 | box2 | box3|   
|------|------|------
| box4 | box5 | box6| 

Well, each line on the sides of the boxes is a mark and determines the beginning or end of the column, the same with the horizontal ones, but the latter are related to the rows. If you want a box to fill a certain space, you must give it some coordinates. For example: We want box2 to pass the second mark and finish in the fourth, therefore, box3 will have to go down one row because box2 will be like:  

| box1 |  box2|  box2  |
|------|------|------|
| box3 | box4 | box5 |
| box6 |
