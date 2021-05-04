# JS : OBJECTs:
##### Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.
+ **VARIABLES BECOME KNOWN AS PROPERTIES**: If a variable is part of an object, it is called a property. Properties te ll us about the object, such as the name of a hotel or the number of rooms it has.
+ **IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS**: If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object.

#### The object is placed in curly braces. It is stored in a variable. 
###### Like variables and named functions, properties and methods have a name and a value. In an object, that name is called a key. An object cannot have two keys with the same name. This is because keys are used to access their corresponding values. The value of a property can be a string, number, Boolean, array, or even another object. The value of a method is always a function.
![image](https://cdn.programiz.com/sites/tutorial2program/files/javascript-object-properties.png)

## Creating An Object: Literal Notation:
###### Literal Notation is the easiest and most popular way to creat objects.
+  **separate each key from it's value using a colon. Separate each property and method with a comma (but not after the last value).**
+ **Treat the values like you would do for variables: Strings live in quotes and Arrays live in square brackets.**

## Accessing An Object and Dot Notation:
###### You can access the properties or methods of an object using Dot Notation. You can also access properties using square brackets.
**To access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method you want to access. 
The period is known as *The member operator*. The property or method on its right is a member of the object on its left. EX: var hotelName = hotel.name;

# JS: Document Object Model (DOM)
##### The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas:
+ **MAKING A MODEL OF THE HTML PAGE**: When the browser loads a web page, it creates a model of the page in memory.
The DOM specifies the way in which the browser should structure this model using a DOM tree. The DOM is called an object model because the model (the DOM tree) is made of objects.
+ **ACCESSING AND CHANGING THE HTML PAGE**: The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.

#### THE DOM TREE IS A MODEL OF A WEB PAGE : It consists of four main types of nodes.
+ **THE DOCUMENT NODE**: At the top of the tree a document node is added; it represents the entire page (and also corresponds to the document object. When you access any element, attribute, or text node, you navigate to it via the document node. It is the starting point for all visits to the DOM tree.

+ **ELEMENT NODES**: To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to.

+ **ATTRIBUTE NODES**: The opening tags of HTML elements can carry attributes. Attribute nodes are not children of the element thar carries them; they are part of that element. Once you access an element, there are specific JavaScript methods and properties to read or change that element's attributes.

+ **TEXT NODES**: Once you have accessed an element node, you
can then reach the text within that element. Text nodes cannot have children. If an element contains text and another child element, the child element is not a child of the text node but rather a child of the containing element.
![image](https://www.researchgate.net/profile/Jian-Chang-8/publication/254002847/figure/fig1/AS:298235726974978@1448116346303/Example-of-DOM-Node-Tree.png)

#### WORKING WITH THE DOM TREE:
**STEP 1: ACCESS THE ELEMENTS : Here is an overview of the methods and properties that access elements.(DOM Queries).
When you need to work with an element more than once, you should use a variable to store the result of this query.**
   + **SELECT AN INDIVIDUAL ELEMENT NODE**: 
       + **get Element Byld ()**: Uses the value of an element's id attribute, This method has one parameter: the value of the id attribute on the element you want to select. This value is placed inside quote marks because it is a string. The quotes can be single or double quotes, but they must match.
       + **querySelector ()**: Uses a CSS selector, and returns the first matching element.
       + You can also select individual elements by **traversing** from one element to another within the DOM tree.

    + **SELECT MULTIPLE ELEMENTS (NODELISTS)**: 
    A Nodelist is a collection of element nodes. Each node is given an index number (a number that starts at zero, just like an array).
       + **getElementsByClassName()**: Selects all elements that have a specific value for their cl ass attribute.
       + **getElementsByTagName()**: Selects all elements that have the specified tag name.
       + **querySelectorAll()**: Uses a CSS selector to select all matching elements.

    + **TRAVERSING BETWEEN ELEMENT NODES**: When you have an element node, you can select another element in relation to it using these five properties.
       + **parentNode**: Selects the parent of the current element node.
       + **previousSibling / nextSibling**: Selects the previous or next sibling from the DOM tree.
       + **firstChild / lastChild**: Select the first or last child of the current element.

**STEP 2: WORK WITH THOSE ELEMENTS**:
  + **ACCESS/ UPDATE TEXT NODES**:
      + Select the (li) element
      + Use the firstChild property to get the text node
      + Use the text node's only property (nodeVa l ue) to get the text from the element
      **nodeValue* This property lets you access or update contents of a text node.**

  + **WORK WITH HTML CONTENT**: 
      + **innerHTML**: One property allows access to child elements and text content.
      + **textContent**: One property allows access to just the text content.

  + **ACCESS OR UPDATE ATTRIBUTE VALUES**: Your choice of techniques depends upon what the element contains.
      + **className /id**: Lets you get or update the value of the class and id attributes.
      + **hasAttribute()**: checks if an attribute exists.
      + **getAttribute()**: gets its value.
      + **setAttribute()**: updates the value.
      + **removeAttribute()**: removes an attribute.

#### Selecting an element from a NodList: 
+ **THE item() METHOD**: Nodelists have a method called item() which will return an individual node from the
Node list. You specify the index number of the element you want as a parameter of the method (inside the parentheses).
Use the length property of the Nodelist - it tells you how many items the Nodelist contains. 
    1. Select elements that have a class attribute whose value is hot and store the Nodelist in a variable called elements.
    2. Use the 1 ength property to check how many elements were found. If 1 or more are found, run the code in the if statement. 
    3. Store the first element from the Node List in a variable called first item. (It says 0 because index numbers start at zero.).

+ **Array Syntax**: You can access individual nodes using a square bracket syntax similar to the array. You specify the index number of the element you want inside square brackets that follow the NodeList.
     1. Creat a NodeList that have a class attribute whose value is (), and store it in a variable.
     2. If that number is greater than or equal to one, run the code inside the if statement.
     3. Get the first element from the NodeList.

#### Repeating Action for an Entire NodeList:
###### You can loop through each node in the collection and apply the same statements to each. It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one.

#### ACCESS & UPDATE A TEXT NODE WITH NODEVALUE:
###### When you select a text node, you can retrieve or amend the content of it using the node Value property. In order to use node Value, you must be on a text node, not the element that contains the text.
 #### ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INNER TEXT):
 ###### The textContent property allows you to collect or update just the text that is in the containing element (and its children).

### Adding Or Removing HTML Content
+ **The innerHTML property**:
     + **Approach**: innerHTML can be used on any element node. It is used both to retrieve and replace replace content.
     + **Adding Content**: 
       1. Store new content as a string in a variable.
       2. Select the elemnt you want to replace its content.
       3. Set the element's innerHTML property to the new string.
    + **Removing Content**: Set innerHTML to an empty string.

+ **DOM Manipulation**: Easily targets individual nodes in the Dom tree.
   + **Approach**: Set of Dom Methods that allow you to creat element and text nodes, and then attach them or remove them from the dome tree.
   + **Adding Content**: You use a dom method to creat a new content, then another dom method to attach it to the right place in the dom tree.
   + **Removing Content**: You can remove an element and any contents and child elements from the dom tree using a single method(removeEl).

### COMPARING TECHNIQUES: UPDATING HTML CONTENT
+ **document.write()**: The document object's write () method is a simple way to add content that was not in the original
source code to the page, but its use is rarely advised.
+ **element.innerHTML**: The innerHTML property lets you get/update the entire content of any element (including markup) as a string.
+ **DOM MANIPULATION**: DOM manipulation refers to using a set of methods and properties to access, create, and update elements and text nodes.

## CROSS-SITE SCRIPTING (XSS) ATTACKS
###### If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise, an attacker could gain access to your users' accounts.

#### HOW XSS HAPPENS:
###### XSS involves an attacker placing malicious code into a site. Websites often feature content created by many different people. 

#### WHAT CAN THESE ATTACKS DO?
###### XSS can give the attacker access to information in:
+ The DOM (including form data)
+ That website's cookies
+ Session tokens: information that identifies you from other users when you log into a site.
**EX**: This example stores cookie data in a variable, which could then be sent to a third-party server:
<(script>var adr= 'http : //example.com/xss .php?cookie=' + escape(document . cookie);</scrip)>

#### DEFENDING AGAINST CROSS-SITE SCRIPTING
###### VALIDATE INPUT GOING TO THE SERVER:
+ 1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation.
+ 2. Double-check validation on the server before displaying user content/storing it in a database.
+ 3. The database may safely contain markup and script from trusted sources. This is because it does not try to process the code; it just stores it.

###### ESCAPE DATA COMING FROM THE SERVER & DATABASE:
+ 4. As your data leaves the database, all potentially dangerous characters should be escaped.
+ 5. Make sure that you are only inserting content generated by users into certain parts of the template files.
+ 6. Do not create DOM fragments containing HTML from untrusted sources. It should only be added as text once it has been escaped.

![image](https://cdn.business2community.com/wp-content/uploads/2019/05/cross-site-scripting-example.png)

## Attribute Nodes
###### You can use other properties and methods to access an element node and change its attribute.
+ **First**, select the element node that carries the attribute and follow it with period symbol.
+ **Then**, Use one of the methods or properties to work with the element's attributes. 
  **Ex**:    getAttribute()  [method]
             class Name      [property] 

#### CHECK FOR AN ATTRIBUTE AND GET ITS VALUES
+ **The hasAttri bute() method of any element node lets you check if an attribute exists. The attribute name is given as an argument in the parentheses.**
+ **ThegetAttribute() method returns the value of the cl ass attribute, which is then written to the page.**

#### CREATING ATTRIBUTES & CHANGING THEIR VALUES
+ **The cl assName property allows you to change the value of the class attribute. If the attribute does not exist, it will be created and given the specified value.**
+ **The setAttri bute() method allows you to update the va lue of any attribute. It takes two parameters: the attribute name, and the value for the attribute.**

#### REMOVING ATTRIBUTES
+ **To remove an attribute from an element, first select the element, then call removeAttribute() . It has one parameter: the name of the attribute to remove.**

![image](https://www.w3schools.com/xml/nodetree.gif)

