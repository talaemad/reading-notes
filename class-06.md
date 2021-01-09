# JS Book

* **Objects** group together a set of variables and functions to create a model of something you would recognize from the real world. In an object, variables and functions take on new names.
* IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
* IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS
* Literal notation is the easiest and most popular way to create objects.
* You access the properties or methods of an object using dot notation. You can also access properties using square brackets.

# Chapter 5
## Document Object Model  (pp.183-242)

* As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.
* Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser.

![Dom tree](https://github.com/talaemad/reading-notes/blob/main/DomTree.png)

* ATTRIBUTE NODES: The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree.
* TEXT NODES: Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node.

* Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

* The terms elements and element nodes are used interchangeably but when people say the DOM is working with an element, it is actually working with a node that represents that element.
* Methods that find elements in the DOM tree are called DOM queries. When you need to work with an element more than once, you should use a variable to store the result of this query.
* When people talk about storing elements in variables, they are really storing the location of elements whin the DOM tree in a variable. The properties and methods of that element node work on the variable.
* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.
* GROUPS OF ELEMENT NODES: If a method can return more than one node, it will always return a Nodelist, which is a collection of nodes (even if it only finds one matching element).
* FASTEST ROUTE: Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive.
* `getElementByld()` and `querySel ector( )`  can both search an entire document and return individual elements. Both use a similar syntax.
`documant.getElementByld()`
* `getElementByld()` allows you to select a single element node by specifying the value of its id attribute.
* A Nodelist is a collection of element nodes. Each node is given an index number (a number that starts at zero, just like an array).
* In a static Nodelist when your script updates the page, the NodeList is not updated to reflect the changes made by the script.
* In a live Nodelist, when your script updates the page, the Nodelist is updated at the same time. The methods beginning getEl ementsBy_ return live Node lists.

* There are two ways to select an element from a Nodelist: The `item()` method and array syntax. Both require the index number of the element you want.
* When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM.
* parentNode: This property finds the element node for the containing (or parent) element in the HTML.
* previousSibling nextSibling: These properties find the previous or next sibling of a node if there are siblings.
* firstChild lastChild: These properties find the first or last child of the current element.
* Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.
* So far this chapter has focused on finding elements in the DOM tree. The rest of this chapter shows how to access/update element content. Your choice of techniques depends upon what the element contains.
* When you select a text node, you can retrieve or amend the content of it using the node Value property.
* The textContent property allows you to collect or update just the text that is in the containing element (and its children).
* `textContent`
To collect the text from the `<li>` elements in our example (and ignore any markup inside the element) you can use the textContent property on the containing `<li>` element. In this case, it would return the value: fresh figs.
* Using the `innerHTML` property, you can access and amend the contents of an element, including any child elements.
* `innerHTML` When getting HTML from an element, the innerHTML property will get the content of an element and return it as one long string, including any markup that the element contains.
* DOM manipulation offers another technique to add new content to a page (rather than innerHTML). It involves three steps:
1. CREATE THE ELEMENT `createElement()` You start by creating a new element node using the `createElement()` method. This element node is stored in a variable.
2. GIVE IT CONTENT: `createTextNode()` createTextNode() creates a  new text node. Again, the node is stored in a variable. It can be added to the element node using the `appendChild()` method.
3. ADD IT TO THE DOM: `appendChild()` Now that you have your element (optionally with some content in a text node), you can add it to the DOM tree using the `appendChi1d()` method.
* DOM manipulation can be used to remove elements from the DOM tree.
* So far, you have seen three techniques for adding HTML to a web page. It's time to compare when you should use each one.
* You can choose different techniques depending on the task (and keep in mind how the site might be developed in the future).
* `element.innerHTML` The innerHTML property lets you get/update the entire content of any element (including markup) as a string.
* If you add HTML to a page using innerHTML (or several jQuery methods), you need to be aware of **Cross-Site Scripting Attacks or XSS**; otherwise, an attacker could gain access to your users' accounts.
* HOW XSS HAPPENS? XSS involves an attacker placing malicious code into a site. Websites often feature content created by many different people.
* Any content generated by users that contain characters that are used in code should be escaped on the server. You must control any markup added to the page.
* ESCAPING USER CONTENT: All data from untrusted sources should be escaped on the server before it is shown on the page. Most server-side languages offer helper functions that will strip-out or escape malicious code.
* Modern browsers come with tools that help you inspect the page loaded in the browser and understand the structure of the DOM tree.
* The browser represents the page using a DOM tree.
* DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
* You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
* Whenever a DOM query can return more than one node, it will always return a Nadelist.
* From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
* An element node can contain multiple text nodes and child elements that are siblings of each other.
* In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
* Browsers offer tools for viewing the DOM tree.