# Html Text and CSS
##### When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

![image](https://i.insider.com/60197cf301504a00197fb20f)
+ **Structural markup**: the elements that you can use to describe both headings and paragraphs.
    * **Headings**: HTML has six "levels" of headings: <h1`>is used for main headings.
    Browsers display the contents of headings at different sizes. The contents of an <h1'> element is the largest, and the contents of an <h6'> element is the smallest.
    * **Paragraphs**: <p'> To create a paragraph, surround the words that make up the paragraph with an opening <p'> tag and closing </p'> tag.
    * **Bold & Italic**: <b'>By enclosing words in the tags  we can make characters appear bold.<b> bold </b>
    <i'> By enclosing words in the tags we can make characters appear italic.<i> italic</i>

+ **Semantic markup**: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it).
    * **Strong & Emphasis**: <strong'> The use of the <strong'> element indicates that its content has strong importance. By default, browsers will show the contents of a <strong'> element in bold.  
    <em'> The <em'> element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an <em'> element in italic.
    * **Quotations**: 1. <blockquote'>: The (blockquote) element is used for longer quotes that take up an entire paragraph. Browsers tend to indent the contents of the (blockquote) element, however you should not use this element just to indent a piece of text.
       2. <q'>: The (q) element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the (q) element, however Internet Explorer does not — therefore many people avoid using the (q) element.
    * **Auth or Details**: <address'>: The (address) element has quite a specific use: to contain contact details for the author of the page. It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address.
    * **Changes to Content**: 1. <ins'>+<del'>: The (ins)element can be used to show content that has been inserted into a document, while the (del) element can show text that has been deleted from it.
      2. <s'>: The (s) element indicates something that is no longer accurate or relevant (but that should not be deleted).
      ![image](http://slidetodoc.com/presentation_image_h/12019ed0a9c51770decb5fba02321ff3/image-17.jpg)

# CSS
##### CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface.

### Understanding CSS:
###### The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element. CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

 **BLOCK & INLINE ELEMENTS**: 
 +  Block level elements look like they start on a new line. Examples include the (h1)-
(h6), (p) and (dev) elements. 
 +  Inline elements flow within the text and do not start on a new line. Examples include (b), (i), (img), (em) and (span).

### CSS Ass ociates Style rules with HTML elements:
###### CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
**EXAMPlE**: (selector)p {font-family: Arial;}(decleration)
+ **Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.
+ **Declarations** indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.
     + **Properties** indicate the aspects of the element you want to change. For example, color, font, width, height and border.
     + **Values** specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.

![image](https://cdn.codecoda.com/themes/user/site/default/asset/img/blog/css-syntax-definition.jpg)  

#### Using External CSS:
**The (link) element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It lives inside the (head) element. It should use three attributes:** 
+ **href** This specifies the path to the CSS file (which is often placed in a folder called css or styles).
+ **type** This attribute specifies the type of document being linked to. The value should be text/css.
+ **rel** This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.

#### Using Internal CSS:
**(style) You can also include CSS rules within an HTML page by placing them inside a (style) element, which usually sits inside the (head) element of the page. When building a site with more than one page, you should use an external CSS style sheet.
![image](https://cf.ppt-online.org/files/slide/k/Kbp3XcismqFREgGuz9OBIWY1vDx6MwHVeZQjC5/slide-8.jpg)

### Why use External Style Sheets?
##### When building a website there are several advantages to placing your CSS rules in a separate style sheet. 
+ **Allows all pages to use the same style rules (rather than repeating them in each page).**
+ **Keeps the content separate from how the page looks.**
+ **Means you can change the styles used across all pages
by altering just one file (rather than each individual page).**
# Javascript
### THE LANGUAGE: SYNTAX AND GRAMMAR
+ **STATEMENTS**: A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.
*var today= new Date();*
   + JAVASCRIPT IS CASE SENSITIVE: age is different than Age.
   + STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE.
   + STATEMENTS CAN BE ORGANIZED INTO CODE BLOCKS.
+ **COMMENTS**: You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.
   + MULTI-LINE COMMENTS: To write a comment that stretches over more than one line, you use a multi-line comment, starting with the /* characters and ending with the * / characters.
   + SINGLE-LINE COMMENTS: In a single-line comment, anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter.
+ **VARIABLES**: A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables. The data stored in a variable can change (or vary) each time a script runs.
    + **How to declare variables?**
    Before you can use avariable, you need to announce that you want to use it. This inclodes creating the variable and giving it a name (declaing the variable). Then you can tell what information you want it to store for you (assign a value to a variable).
    **var age = 26;** 

### DATA TYPES:
###### JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.
![image](https://peinutz.gitbooks.io/javascript/content/assets/import.png)

#### ARRAYS:
###### An array is a special type of variable. It doesn't just store one value; it stores a list of values. You should consider using an array whenever you are working with a list or a set of values that are related to each other. You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array).
  + **array literal**: The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array.
  + **array constructor**:You can also write each value on a separate line. This uses the new keyword followed by Array(); The va lues are then specified in parentheses (not square brackets), and each value is separated by a comma.

#### EXPRESSIONS:
###### An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions.
+ **EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE**:  *var color = 'beige';*
+ **EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE**: *var area = 3 * 2;*

#### OPERATORS:
###### Expressions rely on things called operators; they allow programmers to create a single value from one or more values. 
+ **ARITHMETIC OPERATORS**: 
![image](https://www.devopsschool.com/blog/wp-content/uploads/2020/07/JavaScript-Arithmatic-Operators.png)

+ **STRING OPERATOR**: There is just one string operator: the + symbol. It is used to join the strings on either side of it.

### DECISIONS AND LOOPS:
##### Decision Making:
###### There are often several places in a script where decisions are made that determine which line of the code should run next. Flowcharts can help you plan for these occasions.
![image](https://s3-eu-west-1.amazonaws.com/arisexpress/info_site/flowchart.png)

##### Evaluating Conditions:
###### In order to make a decision, your code checks the current status of the script by comparing two values using a comparison operator Which returns a value of true or false.

##### Conditional Statements: 
###### A conditional statement is based on a concept of if/then/else. If a condition is met, then your code excutes one or more statements, else your code does something different(or just skips the step).
![image](https://i.ytimg.com/vi/wFB-ywsNPwg/maxresdefault.jpg)

##### Logical Operators:
###### comparison operators









