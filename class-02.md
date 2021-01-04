# HTML Book 

## Chapter 2

* HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).
* They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).
* `<b>` and `</b>` we can make characters appear bold.
* `<i>` and `</i>` we can make characters appear italic.
* `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power.
* `<sub>` element is used to contain characters that should be subscript.
* `<br />` to add a line break inside the middle of a paragraph.
* `<hr />` add a horizontal rule between sections
* `<strong>` element indicates that its content has strong importance.
* `<em>` element indicates emphasis that subtly changes the meaning of a sentence.
* `<q>`element is used for shorter quotes that sit within a paragraph.
* `<blockquote>` element is used for longer quotes that take up an entire paragraph.
* `<abbr>` you use an abbreviation or an acronym.
* Semantic information is carried in elements such as `<cite>` and `<em>` .
* `<cite>` When you are referencing a piece of work such as a book, film or research paper.
* The `<dfn>` element is used to indicate the defining instance of a new term.
* `<address>` element has quite a specific use: to contain contact details for the author of the page.
* Note: Browsers often display the content of the `<address>` element in italics.
* `<ins>` element can be used to show content that has been inserted into a document.
* `<del>` element can show text that has been deleted from it.
* Note: The content of a `<ins>` element is usually underlined, while the content of a `<del>`element usually has a line through it.
* `<s>` element indicates something that is no longer accurate or relevant (but that should not be deleted).


## Chapter 10

* CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
* CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon.
Ex. ` p { font-family: Arial;}`
* p (tag name) => Selector
* font-family (style) => Declaration
* font-family(property): Arial(value)

* The `<link>` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. Ex. `<link href="css/styles.css" type="text/css" rel="stylesheet" />`
* The `<style>` element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/ css .

![Selector types in css](https://github.com/talaemad/reading-notes/blob/main/Selector.png)

* When building a website there are several advantages to placing your CSS rules in a separate style sheet.

* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
* Different types of selectors allow you to target your rules at different elements.
* Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document, although they may appear within an HTML page.

# JS Book 

## Chapter 2

* A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.
* You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.
* The variable: values that can generally be accessed or changed at any time.
`var x; ` 
* var => variable keyword, needed to declare the variable
* x => the name of the variable.
` x= value;`
* `=` assignment operator
* the data type of x will be as the value datatype if it was string needed to be between single or double quotes.

* An array is a special type of variable. It doesn't just store one value; it stores a list of values.
* You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array.
`var colors = ['white', 'black', ' custom ' ];`
* index values start at 0 (not 1).
* JavaScript distinguishes between numbers (0 -9), strings (text), and Boolean values (true or false).
* Expressions evaluate into a single value.
* Expressions rely on operators to calculate a value.

## Chapter 4

## Decision Making

The IF statement is the most simple decision-making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statements is executed otherwise not.

There are two components to the decision:
1. An expression is evaluated, which returns a value.
2. A conditional statement says what to do in a given situation.
`if (condition) {...}`
* the condition is an expression if the value of it true the statements between the if block will execute if not (false) they will not.

If there is more than one condition we want to check and each of them had different process we could use if ... else statement.

* `==` =>equal to, compare the value not data type.
* `===`  => strict equal to, compare the value and the data type.
* `!=` => not equal, compare the value not data type.
* `!==`  => strict not equal to, compare the value and the data type.
* `> =`> is greater than, check the left number is greater than the right number. 
* `>=` => greater than or equal to, check the left number is greater or equal to the right number.
* `<`less than, check the left number is less the right number. 
* `<=` less than or equal to, check the left number is less or equal to the right number.

# logical operators

* usually return single values of true or false.
* logical operators allow you to compare the results of more than one comparison operator.
* `&&` => logical and, test more than one condition, return true when both expressions true.
* `||` => logical or, test at least one condition, return true always except when both false return false.
* `!` => logical not, takes a single boolean value and inverts it.
