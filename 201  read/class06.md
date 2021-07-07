# WHAT IS AN OBJECT? 
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 

- IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES.
- IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS.

![image](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/How-to-Create-JavaScript-Objects.jpg)

## Example for object :
 
 ![image](https://miro.medium.com/max/1844/1*Nqr_lGr3L42az-Pde_AtsQ.png)

 ![image](https://image1.slideserve.com/3013700/creating-objects-using-literal-notation-l.jpg)

# Document Object Model
The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

## THE DOM TREE IS A MODEL OF A WEB PAGE

![image](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Js-Dom-Tree.png)

## WORKING WITH THE DOM TREE

1. ACCESS THE ELEMENTS 
   - SELECT AN INDIVIDUAL ELEMENT NODE
   - SELECT MULTIPLE ELEMENTS (NODELISTS)
   - TRAVERSING BETWEEN ELEMENT NODES

2. WORK WITH THOSE ELEMENTS
   - ACCESS/ UPDATE TEXT NODES
   - WORK W ITH HTML CONTENT
   - ACCESS OR UPDATE ATTRIBUTE VALUES

# summary

1. The browser represents the page using a DOM tree.
2. DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
3. You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
4. Whenever a DOM query can return more than one node, it will always return a Nade list.
5. From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
6. An element node can contain multiple text nodes and child elements that are siblings of each other.
7. In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
8. Browsers offer tools for viewing the DOM tree . 