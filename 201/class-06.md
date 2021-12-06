<h3>Object Literals</h3>
<ol>
<li>Objects are made up of properties, which are key value pairs</li>
<li>Populating objects: separate each key-value pair with a comma</li>
<li>properties that are functions are called methods</li>
<li>if accessing/changing a prop, use dot notation, if accessing props via function, use bracket notation </li>
</ol>
<h3>Document Object Model: DOM</h3>
<ol>
<li>DOM trees are a model of the webpage: It consists of 4 different types of nodes: 
  <ol>
  <li>Document node: document object</li>
  <li>Element node: html elements</li>
  <li>Attribute node: element attributes</li>
  <li>Text node: the text within elements</li>
  </ol>
  </li> 
  <br>
  Methods that find elements in the DOM tree are called DOM queries.
  <br> <br> When people talk about storing elements in variables, they are really storing the location of the element(s) within the DOM tree in a variable.

<br><li>Accessing elements in DOM trees
  <ol>
   <li>You must access the methods via the document object (i.e document.getElementById()</li>
   <li>Selecting an individual element:</li>
    <ol>
    <li>getElementById() Uses the el's id</li>
    <li>querySelector() Uses CSS selector and returns first matching el</li>
    </ol>
   <li>Selecting multiple elements(Node lists)
    <ol>
    <li>getElementsByClassName() </li>
    <li>getElementsByTagName()</li>
    <li>querySelectorA11() Use CSS selector to get all matching elements</li>
    </ol>
   </li>
   <li>Traversing between element nodes:
    <ol>
    <li>parentNode: Selects the parent of the current el node</li>
    <li>previousSibling/nextSibling: Selects the previous/next sibling on the DOM tree</li>
    <li>firstChild/lastChild: Selects the firstChild/lastChild of the element</li>
    </ol>
   </li>
  </ol>
</li>
<li>Fastest Route: Finding the fastest way to access an element within your webpage will make it seem faster/more responsive; usually the fastest way to access a singular element is getElementById()</li>
</ol>
