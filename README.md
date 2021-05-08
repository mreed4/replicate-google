# Google Homepage

## The Project

Per the [instructions](https://www.theodinproject.com/paths/foundations/courses/foundations/lessons/html-css) on the Odin Project, I am to essentially replicate the appearance (but not necessarily the functionality) of the main Google page (the one with the search box, the logo, and not much else).

The instructions and/or the "rules" are to:

1. Add the logo and the search box

2. Add the navbar

3. Add the footer

4. Do as much as possible without using the browser's developer tools and without viewing the source code

5. Do not "cheat" by looking at the solutions by other Odin students before you complete your attempt

6. It does not have to be pixel perfect

## Notes and Challenges

I found myself using both knowledge learned from Odin, as well as pre-existing knowledge I had from a time I taught myself HTML and CSS about 10+ years ago. This was a time before flexbox, before Bootstrap (or before it was so big, or so well known), and of course before Odin.

I ran into some challenges however.

### The Search Icon

A current challenge I am facing is that--on Google's actual site--the magnifying glass icon "in" the search box is a gray color. In my project, while I *am* using the Material Design icons provided by Google, the icon is black, not gray.

The manner in which I added the icon to the search box in my project[^1] does not allow me to use pure code to alter the color of the image.

Without looking at the source code, I am not sure of the solution that Google used. Did they (a) add it as an image in the HTML (i.e. using `<img>` not `background: <code>`) and used pure CSS code (e.g. `img {opacity: <code>}`) to alter the image, or did they (b) they alter the image in an external program, then use the altered image in the HTML?

### The Footer

While the navbar looks simple enough, the footer has several items in it, seemingly split into two rows (when viewed below a certain viewport width).

When the viewport is increased beyond a certain size  however, the two rows become one row, and the single item formerly appearing in the top row is added to the center of what was the bottom row.

My *guess* is that this is the result of the magic of flexbox or CSS grid and responsive design (and this is the solution I plan to use), but time will tell.

[^1]: I did this using CSS' `background: <code>` and `padding: <code>` property(ies)
