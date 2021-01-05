# HTML Book

## Chapter 4

* Links are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute.
* `<a href="url">The-Name</a>` 
* Absolute URLs :When linking to other. For example link to google.
* Relative URLs : When linking to other pages within the same site, you can use relative URLs.
* On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.
* Structure: The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts.
* Relationships: The relationship between files and folders on a website is described using the same terminology as a family tree.
* Homepages: The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called index.htm.
* Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.
![relative types](https://github.com/talaemad/reading-notes/blob/main/Relative.png)

* Email Links: To create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>` element. However, this time the value of the href attribute starts with `mailto:` and is followed by the email address you want the email to be sent to.
* `<a href="mailto:Name@example.org">Name-Email</a>`
* Opening Links in a New Window: If you want a link to open in a new window, you can use the `target` attribute on the opening `<a>` tag. The value of this attribute should be _blank.
* `<a href="url" target="_blank">`
* To link to an element that uses an `id` attribute you use the `<a>` element again, but the value of the href attribute starts with the `#` symbol, followed by the value of the `id` attribute of the element you want to link to. 
 `<h1 id="top">TEXT</h1>`
 `<a href="#top">Top</a>`
* Links are created using the <a> element.
* The <a> element uses the href attribute to indicate the page you are linking to.
* If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
* You can create links to open email programs with an email address in the "to" field.
* You can use the id attribute to target elements within a page that can be linked to.

## Chapter 15

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


# JS Book

## Chapter 3

* Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements.
* To create a Function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a function declaration.
* Calling Function: you can then execute all of the statements between its curly braces with just one line code.
* Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it parameters. Inside the function, the parameters act like variables.
* when you call a function that has parameters, you specify the values it should use in the parentheses that follow its name. The values are called arguments, and they can be provided as values or variables.
* some functions return information to the code that called them. For example, when they perform calculations, they return the result.
* Functions can return more than one value using an array. For example, this function calculates the area and volume of a box.
* Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression.
* The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.
* Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.
* CREATING THE VARIABLES IN CODE: Each variable that you declare takes up memory. The more va ri ables a browser has to remember, the more memory your script requires to run. Scripts that require a lot of memory can perform slower, which in turn makes your web page take longer to respond to the user.
* NAMING COLLISIONS: You might think you would avoid naming collisions; after all you know which va riables you are using. But many sites use scripts written by several people. If an HTML page uses two JavaScript files, and both have a global variable with the same name, it can cause errors. Imagine a page using these two scripts.


* pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together. At Code Fellows, pair programming is one way we foster a collaborative environment while developing key industry skills.

* pair programming commonly involves two roles: the Driver and the Navigator. The driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the coding. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer.

* Pair programming touches four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

## 6 Reasons for Pair Programming

1. Greater efficiency
when two people focus on the same code base, it is easier to catchmistakes in the making. Research indicates that pair programmingtakes slightly longer, but produces higher-quality code that doesn’trequire later effort in troubleshooting and debugging.
2. Engaged collaboration
It is harder to procrastinate or get off track when someone else is relying on you to complete the work.
Another important aspect of learning to program is knowing when to ask for help.
3. Learning from fellow students
Everyone has a different approach to problem-solving; working with a teammate can expose developers to techniques they otherwise would not have thought of.
4. Social skills
When working with someone who has a different coding style,communication is key. This can become more difficult when twoprogrammers have different personalities. 
5. Job interview readiness
They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing codebase.
6. Work environment readiness
Many companies that utilize pair programming expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.