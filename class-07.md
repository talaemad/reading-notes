# Domain Modeling
* Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.
* Here's some tips to follow when building your own domain models.

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.
# HTML Book
# Chapter 6: “Tables” (pp.126-145)
* A table represents information in a grid format.
* `<table>` The `<table>` element is used to create a table. The contents of the table are written out row by row.
* `<tr>` You indicate the start of each row using the opening `<tr>` tag. (The tr stands for table row.)
* `<td>` Each cell of a table is represented using a `<td>` element. (The td stands for table data.)
* The `<th>` element is used just like the `<td>` element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)
* Spanning Columns: The colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across.
* `<thead>` The headings of the table should sit inside the `<thead>` element.
* `<tbody>` The body should sit inside the `<tbody>` element.
* `<tfoot>` The footer belongs inside the `<tfoot>` element.

* The `<table>` element is used to add tables to a web page.
* A table is drawn out row by row. Each row is created with the `<tr>` element.
* Inside each row there are a number of cells represented by the `<td>` element (or `<th>` if it is a header).
* You can make cells of a table span more than one row or column using the rowspan and colspan attributes.
* For long tables you can split the table into a `<thead>`, `<tbody>`, and `<tfoot>`.
# JS Book
# Chapter 3: “Functions, Methods, and Objects” (pp.106-144)
* Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods. 
* Once you have created an object (using literal or constructor notation), you can add new properties to it.
* CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS
* the object is created on the first line of the code sample. The properties and methods are then added to it afterwards.
* Once you have created an object, the syntax for adding or removing any properties and methods from that object is the same.
* LITERAL NOTATION A colon separates the key/value pairs. There is a comma between each key/value pair.
* OBJECT CONSTRUCTOR NOTATION The function can be used to create multiple objects. The this keyword is used instead of the object name.
* The keyword `this` is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.
* A FUNCTION IN GLOBAL SCOPE When a function is created at the top level of a script (that is, not inside another object or function), then it is in the global scope or global context.
* GLOBAL VARIABLES All global variables also become properties of the window object. so when a function is in the global context, you can access global variables using the window object, as well as its other properties.
* In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.
* If you want to access items via a property name or key, use an object (but note that each key in the object must be unique). If the order of the items is important, use an array.
* Arrays are acutely speacial type of object.
* you can combine array and object.
* Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages. 
* The window object represents the current browser window or tab. It is the topmost object in the Browser Object Model, and it contains other objects that tell you about the browser.
* In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).
* Whenever you have a value that is a number, you can use the methods and properties of the Number object on it.
* The Math object has properties and methods for mathematical constants and functions.
* JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.