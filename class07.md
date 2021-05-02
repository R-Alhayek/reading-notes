# Domain Modeling
###### Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

**Here are some tips to follow when building your own domain models.**
 1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
 2. Model its attributes with a constructor function that defines and initializes properties.
 3. Model its behaviors with small methods that focus on doing one job well.
 4. Create instances using the new keyword followed by a call to a constructor function.
 5. Store the newly created object in a variable so you can access its properties and methods from outside.
 6. Use the this variable within methods so you can access the object's properties and methods from inside.

# Html: Tables 
###### There are several types of information that need to be displayed in a grid or table. For example: sports results, stock reports, train timetables. In HTML a table is written out row by row.
![image](https://ictacademy.com.ng/wp-content/uploads/2017/10/HTML-Table-Structure.png)

#### Basic Table Structure
+ **(table)**: The (table) element is used to create a table. The contents of the table are written out row by row.
+ **(tr)**: You indicate the start of each row using the opening (tr) tag. (The tr stands for table row.) It is followed by one or more (td) elements (one for each cell
in that row). At the end of the row you use a closing (/tr) tag.
+ **(td)**:Each cell of a table is represented using a (td) element. (The td stands for table data.) At the end of each cell you use a closing (/td) tag.

#### Table Headings
+ **(th)**: The (th) element is used just like the (th) element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.) Even if a cell has no content, you should still use a (th) or (th) element to represent the presence of an empty cell otherwise the table will not render correctly.

#### Spanning ColumnS and Rows
+ **The colspan attribute** can be used on a (th) or (td) element and indicates how many columns that cell should run across.
+ **The rowspan attribute** can be used on a (th) or (td) element to indicate how many rows a cell should span down the table.

#### Long Tables
###### There are three elements that help distinguish between the main content of the table and the first and last rows. These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table.
+ **(thead)**: The headings of the table should sit inside the (thead) element.
+ **(tbody)**: The body should sit inside the (tbody) element.
+ **(tfoot)**: The footer belongs inside the (tfoot) element.

### Old Code:
##### Width & Spacing:
###### The width attribute was used on the opening (table) tag to indicate how wide that table should be and on some opening (th) and (td) tags to specify the width of individual cells. The value of this attribute is the width of the table or cell in pixels.
###### The opening (table) tag could also use the cellpadding attribute to add space inside each cell of the table, and the cellspacing attribute to create space between each cell of the table. The values for these attributes were given in pixels.

##### Border & Background
###### The border attribute was used on both the (table) and (td) elements to indicate the width of the border in pixels.
###### The bgcolor attribute was used to indicate background colors of either the entire table or individual table cells. The value is usually a hex code.

# JS : Creating An Object/ Constructor Notation
###### The **new** keyword and the **object** constructor creat a blank object. You can then add properties and methods to that object.
+ **First**, You creat a new object using a combination of the new key word and the object constructor function.
+ **Next**, in this blank object you can add properties and methods using dot notation. Each statement should end with semicolon.
##### CREATING AN OBJECT WITH PROPERTIES & METHODS
+ **LITERAL NOTATION**: A colon separates the key/value pairs. There is a comma between each key/value pair.
+ **OBJECT CONSTRUCTOR NOTATION**: The function can be used to create multiple objects. The **this** keyword is used instead of the object name.

## Updating An Object
+ **To update the value of properties, use dot notation or square brackets but with a new value.**
+ **To delete a property, use the **delete** keyword.**

## Creating Many Objects: Constructor Notation
###### Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods.
+ The **this** keyword is used instead of the object name to indicate that the property or method belongs to the object that this function creates. Each statement that creates a new property or method for this object ends in a semicolon.

+ The name of a constructor function usually begins with a capital letter (unlike other functions, which tend to begin with a lowercase character). 

## THIS KEYWORD
###### The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

## Arrays 
###### Arrays are actually a special type of objects.They hold a related set of keys/values pairs, but the key for each value is its index number.

#### Arrays of objects & objects in arrays
###### You can combine arrays and objects to creat complex data structure.
+ **Arrays in an objects**: The property of any object can hold an array.
+ **Object in an array**: The value of any element in an array can be an object.
![image](https://soshace.com/wp-content/uploads/2020/08/cover_1200x630.jpg)

## Built-in Objects
+ **Browser Object Model/THE WINDOW OBJECT**: It creats a model of the browser tab or window. It is the topmost object in the Browser Object Model, and it contains other objects that tell you about the browser.
**EX**: window . innerHeight: Height of window (excluding browser chrome/user interface) (in pixels)
+ **THE DOCUMENT OBJECT MODEL: THE DOCUMENT OBJECT**: The topmost object in the Document Object Model (or DOM) is the document object. It represents the web page loaded into the current browser window or tab.
**EX**: document.title :Title of current document.
+ **GLOBAL Javascript OBJECTS: They are a group of individual objects that relate to different parts of the javascript language. Their names usually starts with a capital letter.
    + **STRING OBJECT**: Whenever you have a value that is a string, you can use the properties and methods of the String object on that value. These properties and methods are often used to work with text stored in variables or objects.
    **EX**: toUpperCase (): Changes string to uppercase characters
    + **NUMBER OBJECT**: Whenever you have a value that is a number, you can use the methods and properties of the Number object on it. 
    **EX**: i sNaN (): Checks if the value is not a number.
    ##### COMMONLY USED TERMS:
    • An **integer** is a whole number (not a fraction).
    • A **real number** is a number that can contain a fractional part.
    • A **floating point number** is a real number that uses decimals to represent a fraction. The term floating point refers to the decimal point.
    • **Scientific notation** is a way of writing numbers that are too big or too small to be convenient ly written in decimal form. For example: 3,750,000,000 can be represented as 3.75 x109 or 3.75e+12.

    + **MATH OBJECT**: The Math object has properties and methods for mathematical constants and functions.
    **EX**: Math. round(): Rounds number to the nearest integer.

    + **DATE OBJECT (AND TIME)**: To work with dates, you creat an instance of the date object. You can then specify the date and time you want it to represent. By defualt, it will hold today's date and current time.
    **EX**: getDate() /setDate(): Returns I sets the day of the month (1-31).
    
    ![image](https://miro.medium.com/max/1988/1*qsMBvORdk1r82DRKZ17gLQ.png)

## DATA TYPES
###### In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).
  + **Simple (or primitive) data types:**
       1. String
       2. Number
       3. Boolean
       4. Undefined: (a variable that has been declared, but no value has been assigned to it yet)
       5. Null: (a variable with no value - it may have had one at some point, but no longer has a value).

  + **COMPLEX DATA TYPE**:
       6. Object: Under the hood, arrays and functions are considered types of objects.

