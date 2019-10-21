# Fundamentals of responsive web design

## First, look at the queries.

Media queries are a solution to adapt the content of the page according to the device you are using.
For example, you want to show some content in a certain way depending on the width or if the device is in "landscape" or "portrait" mode.

## Responsive image

You can achieve a responsive image doing the following set up:
- Assign a max-width property of 100%, like that, you can cover the container but ensure that the image doesn't expand.
- Then, display the img tag as a block element.
- Last, put the height in auto, this will ensure the aspect ratio of the image.

## Use the retina trick

Some devices has a higher pixel density that others, and willing to achieve the correct display of the content, we only have to reduce the width and height to the half of its original stats.

## Typography that adapts 

When we are building a website, we want all users to see the page correctly, regardless of the device they are using and the typography within the text does not escape that idea. The solution here is to use relative units (mainly vmin, vmax, vh and vw). They differ from absolute units in the way they behave. The latter does not change the way it is displayed and the first uses the dimensions of the viewport (in simple words, it is the screen where the content is displayed) to adapt the size of the text. For example, if the viewport changes its width and we can tolerate a reduce on the font-size, if so, the only thing we have to do is assign to the font-size property a value of "x" vw where x is a positive number and represent a % of the total width of the viewport.
