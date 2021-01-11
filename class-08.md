# HTML Book
# Chapter 15: Layout

* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
* Block-level elements start on a new line Examples include: `<h1>` `<p>` `<ul>` `<li>`
* Inline elements flow in between surrounding text Examples include: `<img>` `<b>` `<i>`
* If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
* A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.
* CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.
* Normal flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.
* Relative Positioning: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
* Absolute positioning: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up).
* Fixed Positioning: This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.
* Floating Elements: Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.
* Relative positioning moves an element in relation to where it would have been in normal flow. `position:relative`
* Fixed positioning: is a type of absolute positioning that requires the position property to have a value of fixed. `position:fixed`
* The `float` property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.
* A lot of layouts place boxes next to each other. The float property is commonly used to achieve this.
* The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:`left` `right` `both` `none`.
* Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.
* Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.
* Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).
* Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
* Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.
* To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too).
* Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers.
* CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.
* `<div>` elements are often used as containing elements to group together sections of a page.
* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right of the page and can be used to create multi-column.
layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts.
* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.