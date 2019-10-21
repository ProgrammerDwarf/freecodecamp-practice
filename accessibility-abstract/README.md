# Elements in the semantic model

## The header tag

Given that some people need to use screen readers and some other tools to get the information on our page. The header has an important task. First, it serves as the introduction of what will be a menu or information that people generally use to find pages on our site.
Second, it serves like an element that will be part of a template for the static sites generators.

## The main tag

The main tag serves to surround the important and main information (yes, you guessed it). It is recommended to only have one tag per page.

## The article tag

This tag is used for content that has its own meaning, does not depend on the context and if you take it from the page it does not lose the meaning

## The section tag

Similar to article but this serves like an element from a collection, doing groups with a commom theme or subject.
The example used for learning was this: "If an article is a book, the sections are the chapters.

## The footer tag

It's like the header, but it contains the content that will guide you to related content or information about site owners, restrictions, licensing and things that users generally don't want to see at first sight of the site.

## The audio tag

As the title says, it serves as a component to listen to an audio track. If you set the `controls` attribute, you will place buttons to control the audio, such as playback, pause and progress bar.

## The figure and figcaption

This duo is excellent to put an image and a brief explaniation to the screen readers of the image. The `figcaption` goes inside the `figure` tag.

## The label and Input

Another duo that enhances the user experience, the "tag" tag serves as a title that wraps up another form element, such as the "input" tag. The input tag use its description in the tag "label" and when a user wishes to select the input field, all they have to do is click on it. To get a better use of this, we put the "for" property with the same name that the identification put before on the input tag something like this:

`<form>`
  `<label for="name">Name:</label>`
  `<input type="text" id="name" name="name">`
`</form>`

## the fieldset and Legend

Again, another duo. When we want to have a lot of options when we make a form, such as radio buttons and we expect the user to select an option on them (or several). If the option is not self-explanatory and we have to use the "fieldset" tag to group the elements and use a legend that serves as a title to explain what those buttons are and what you are enabling when you select them.

## The time tag and datetime attr

You can hold dates with this inline tag, the "datetime" attribute state a valid format for a date, this is for the assistive devices.

## Readability and contrast

Taken from the explanation on the FCC curriculum "The Web Content Accessibility Guidelines (WCAG) recommend at least a 4.5 to 1 contrast ratio for normal text. The ratio is calculated by comparing the relative luminance values of two colors. This ranges from 1:1 for the same color, or no contrast, to 21:1 for white against black, the strongest contrast. There are many contrast checking tools available online that calculate this ratio for you."

## The accesskey attribute and tabindex

The `accesskey` attr does a shortcut to the link or button (in fact, all the elements can use this attr) a user wants to reach with the keyboard.  
Similar to it, we have the tabindex attr. It does nearly the same but it focus an element and is reached with the tab key in an order that began from 1 to whichever positive number you use. The negative numbers that would be used means that you can focus that element but you can't reach it with the keyboard.  
