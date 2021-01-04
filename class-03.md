#  HTML Book
## Chapter 3
* The ordered list is created with the `<ol>` element.
* Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag.
* The unordered list is created with the `<ul>` element.
* Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag.
* The definition list is created with the `<dl>`.
* ` <dt>` to contain the term being defined.
* `<dd>` This is used to contain the definition.
* There are three types of HTML lists: ordered, unordered, and definition.
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another.

## Chapter 13

* Every box has three available properties that can be adjusted to control its appearance: Border,Margin,Padding.
* If you specify a width for a box, then the borders, margin, and padding are added to its width and height.
* The padding and margin properties are very helpful in adding space between various items on the page.
* The border-width property is used to control the width of a border with following values:thin, medium, thick.
* The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can.
* inline This causes a block-level element to act like an inline element.
* block This causes an inline element to act like a block-level element.
* inline-block This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
* none This hides an element from the page. In this case, the element acts as though it is not on the page at all (although a user could still see the content of the box if they used the view source option in their browser).
* hidden This hides the element.
* visible This shows the element.
* CSS treats each HTML element as if it has its own box.
* You can use CSS to control the dimensions of a box.
* You can also control the borders, margin and padding for each box with CSS.
* It is possible to hide elements using the display and visibility properties.
* Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
* Legibility can be improved by controlling the width of boxes containing text and the leading.
* CSS3 has introduced the ability to create image borders and rounded borders.

#  JS Book
##  Chapter 2

* An array is a special type of variable. It doesn't just store one value; it stores a list of values.
* You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array.
`var colors = ['white', 'black', ' custom ' ];`
* index values start at 0 (not 1).
* JavaScript distinguishes between numbers (0 -9), strings (text), and Boolean values (true or false).
* Expressions evaluate into a single value.
* Expressions rely on operators to calculate a value.

## Chapter 4

* A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 
* You have a default option that is run if none of the cases match.
* If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple i f statements). 
* If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error.
* Due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects.  
* Because the presence of an object or array can be considered truthy, it is often used to check for the existence of an element within a page.

* loop types:
**For** => use it if you know how much time you need to run the code.
**While** => use it if you don't how many times the code needs to run.
**Do While** => it will always run time, even if the condition is false from the beginning.

* For loop: use counter as condution.(initialization `var i=0 `,condition `i<value` ,update`i++`)
* in every loop it need to check the condition and update the value. it will end looping when condition return false.

* while loop: This loop will continue to run for as long as the condition in the parentheses is true.

* Conditional statements allow your code to make decisions about what to do next.
* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands.
* Logical operators allow you to combine more than one set of comparison operators.
* if ... else statements allow you to run one set of code if a condition is true, and another if it is false.
* switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).
* Data types can be coerced from one type to another.
* All values evaluate to either truthy or falsy.
* There are three types of loop: for, while, and do ... while. Each repeats a set of statements. 