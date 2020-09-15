# Layout
## Building Blocks
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box
- Block-level elements : 
start on a new line ```<h1> <p> <ul> <li>```
- Inline elements :
flow in between surrounding text ```<img> <b> <i>```
## Containing Elements
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.

## Controlling the Position of Elements
- positioning schemes
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.
1. Normal flow
2. Relative Positioning
3. Absolute positioning
## box offset 
 properties used  to tell the browser how far from the top or bottom and left or right it should be placed. 
- Fixed Positioning 
- Floating Elements
> When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.
## Screen Sizes
Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to
work on a range of different sized screens.
## Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens
## Page Sizes
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide
## Fixed Width Layouts
- Advantages
1. Pixel values are accurate at controlling size and positioning of elements.
2. The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
3. You can control the lengths of lines of text regardless of the size of the user's window.
- Disadvantages
1.  You can end up with big gaps around the edge of a page.
2. If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
3. If a user increases font sizes, text might not fit into the allotted spaces.


> Grids help create professional and flexible designs.

> CSS Frameworks provide rules for common tasks.

> You can include multiple CSS files in one page.
