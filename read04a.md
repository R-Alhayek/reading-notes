# Writing script for a web page.
#### When creating a web page, developers usually use three languages; **HTML**, **CSS**, **Javascript**. Each language forms a separate    layer with a different purpose. 
+ **HTML** : This is where the content of the page lives. The HTML           gives the page structure and adds semantics. 
+ **CSS** : The CSS enhances the HTML page with rules that state how 
       the HTML content is presented (backgrounds, borders, box 
       dimensions, colors, fonts, etc.). 
+ **Javascript** : This is where we can change how the page behaves, adding interactivity. 
![image](https://miro.medium.com/max/3840/0*crN1sMRpNnApF9Pe.png)

## CREATING A BASIC JAVASCRIPT.
#### JavaScript is written in plain text, just like HTML and CSS, so you do not need any new tools to write a script.
+ Create a folder and put the Javascript file in.
+ Open your HTML page and insert the The HTML <script> element at the end of the body, which is used to load the JavaScript file into the page. It has an attribute called src, whose value is the path to the script you created.This tells the browser to find and load the script file.
+ Now you can enter the javascripts you want and test them.


## Basic Javascript Elements.
#### like any new language, there are new words to learn (the vocabulary) and rules for how these can be put together (the grammar and syntax of the language). 
#### Web browsers (and computers in general) approach tasks in a very different way than a human might. Your instructions need to reflect how computers get things done. 
+ **STATEMENTS** :A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon.Some statements are surrounded by curly braces; these are known as code blocks. The closing curly brace is not followed by a semicolon. 
+ **COMMENTS** : You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. 
  + JavaScript code is green 
  *Multi-line* comments are pink 
  *Single-line* comments are gray 
+ **VARIABLE** : A script will have to temporarily store the bits of information it needs to do its job in variables which tell the interpreter every individual step that you want it to perform. So, *VARIABLES* are used "remember" the values and the data stored in a variable can change (or vary) each time a script runs. 

![image](https://datavisioner.net/wp-content/uploads/2020/04/javascript-illustration.png)


## DATA TYPES.
#### JavaScript distinguishes between numbers, strings, and true or false values known as Booleans. 
+ **NUMERIC DATA TYPE** : The numeric data type handles numbers. For tasks that involve counting or calculating sums, you will use numbers 0-9. You can also have negative numbers.
+ **STRING DATA TYPE** : The strings data type consists of letters and other characters. the string data type is enclosed within a pair of quotes. These can be single or double quotes. Strings are frequently used to add new content into a page and they can contain HTML markup.
+ **BOOLEAN DATA TYPE** : Boolean data types can have one of two values: true or false. 

## RULES FOR NAMING VARIABLES.
1. The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number. 
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). 
3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something.
4. All variables are case sensitive, so it is bad practice to create two variables that have the same name using different cases. 
5. Use a name that describes the kind of information that the variable stores.
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word. For example, firstName rather than firstname.
 
![image](https://tutorial.techaltum.com/images/js-variables.jpg)