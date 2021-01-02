# HTML Book

## Introduction

**How the Web Work:**

* When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site; for example: google.com.
* Your computer contacts a network of servers called Domain Name System (DNS) servers. They tell your computer the IP address associated with the requested domain name. Every device connected to the web has a unique IP address; it is like the id for that computer.
* The IP address that the DNS server returns to your computer allows your browser to contact the webserver that hosts the website you requested.
* The web server then sends the page you requested back to your web browser.

### Definition

* Web Server: is a computer that is constantly connected to the web and is set up especially to send web pages to users.
* An IP address is a number of up to 12 digits separated by periods / full stops.

## Chapter 1

* HTML pages are text documents.
* HTML uses elements to describe the structure of pages.
* There are several different elements in HTML, each element has an opening tag and a closing tag.
* Tags act like containers. They tell you something about the information that lies between their opening and closing tags.
* Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equal sign.
` <p color="red"> `

## Chapter 8

* DOCTYPES tell browsers which version of HTML you are using.
* You can add comments to your code between the ` <!-- and --> ` markers.
* The id and class attributes allow you to identify particular elements.
* The ` <div> ` and ` <span> ` elements allow you to group block-level and inline elements together.
* ` <iframe>` An iframe is like a little window that has been cut into your page — and in that window, you can see another page. The term iframe is an abbreviation of an inline frame.
* The ` <meta> ` tag allows you to supply all kinds of information about your web page.
* There are some characters that are used in and reserved by HTML code. (For example, the left and right-angled brackets.). For that, if you want these characters to appear on your page you need to use what are termed "escape" characters.

![escape-characters](https://github.com/talaemad/reading-notes/blob/main/chr.png)


## Chapter 17

* The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
* The new elements provide clearer code (compared with using multiple `<div>` elements).
* Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
* To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

## Chapter 18

* It's important to understand who your target audience is, why they would come to your site, what information they want to find, and when they are likely to return.
* Site maps allow you to plan the structure of a site.
* Wireframes allow you to organize the information that will need to go on each page.
* Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
* You can differentiate between pieces of information using size, color, and style.
* You can use grouping and similarity to help simplify the information you present.

# JS Book

* Once you know the goal of your script, you can work out the individual tasks needed to achieve it.
* Each individual task may be broken down into a sequence of steps.
* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task programmatically.
* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help).

### HOW A BROWSER SEES A WEB PAGE

* RECEIVE A PAGE AS HTML CODE
* CREATE A MODEL OF THE PAGE AND STORE IT IN MEMORY.
* USE A RENDERING ENGINE TO SHOW THE PAGE ON SCREEN.

* It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the `.js` extension.
* The HTML `<script>` element is used in HTML pages to tell the browser to load the JavaScript file (rather like the `<link>` element can be used to load a CSS file).
* If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created.