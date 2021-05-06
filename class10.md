# JS: Error Handling & Debugging
###### When you are writing JavaScript, do not expect to write it perfectly the first time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too.

#### ORDER OF EXECUTION
###### The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run. You might think that the order of execution (the order in which statements are processed) would be as numbered: one through to four. However, it is a little more complicated. To complete step one, the interpreter needs the results of the functions in steps two and three (because the message contains values returned by those functions). The order of execution is more like this: 1, 2, 3, 2, 1, 4.

#### EXECUTION CONTEXTS
+ **GLOBAL CONTEXT**: Code that is in the script, but not in a function. There is only one global context in any page.
+ **FUNCTION CONTEXT**: Code that is being run within a function. Each function has its own function context.
+ **EVAL CONTEXT (NOT SHOWN)**: Text is executed like code in an internal function called eva l ().

+ **VARIABLE SCOPE**: 
     + **GLOBAL SCOPE**: If a variable is declared outside a function, it can be used anywhere because it has global scope.
     + **FUNCTION-LEVEL SCOPE**: When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

### The Stack
###### The Java Script interpreter processes one line of a code at a time.When a stetement has to call some other code in order to its job, the new task goes to the top of the pile of things to do. Once the new task has been performed, the interpreter can go back to the task in hand.

#### EXECUTION CONTEXT & HOISTING
+ **1: PREPARE**: 
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined

+ **2: EXECUTE**:
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements
###### The preparation phase is often described as taking all of the variables and functions and hoisting them to the top of the execution context. Or you can think of them as having been prepared. Each execution context also creates its own vari ab 1 es object. This object contains details of all of the variables, functions, and parameters for that execution context.

#### UNDERSTANDING SCOPE
###### In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

#### UNDERSTANDING ERRORS
###### If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.
**If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error (you meet them on p480). This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.**

#### ERROR OBJECTS
###### Error objects can help you find where your mistakes are and browsers have tools to help you read them.
![image](https://d2gg9evh47fn9z.cloudfront.net/800px_COLOURBOX24249364.jpg)

#### Syntax Error:
+ **SYNTAX IS NOT CORRECT**: This is caused by incorrect use of the rules of the language. It is often the result of a simple typo.
+ **Unexpected EOF**: MISMATCHING OR UNCLOSED QUOTES.
+ **SyntaxErr or : Expected token ' ) '**: MISSING CLOSING BRACKET.
+ **SyntaxError: Expected token ']'**: MISSING COMMA IN ARRAY.

#### Reference Error:
+ **VARIABLE DOES NOT EXIST**: This is caused by a variable that is not declared or is out of scope.
+ **ReferenceError: Can't find variable : randomFunction**: NAMED FUNCTION IS UNDEFINED.

#### EvalError
+ **INCORRECT USE OF eval() FUNCTION**: The eva l () function evaluates text through the interpreter and runs it as code.

#### URI Error
+ **INCORRECT USE OF URI FUNCTIONS**: If these characters are not escaped in URls, they will cause an error: / ? & I : ;

### HOW TO DEAL WITH ERRORS
+ **1: DEBUG THE SCRIPT TO FIX ERRORS**: If you come across an error while writing a script, you will need to debug the code, track down the source of the error, and fix it. The developer tools available in every major modern browser will help you with this task. 
+ **2: HANDLE ERRORS GRACEFULLY**: You can handle errors gracefully using try, catch, throw, and finally statements. Sometimes, an error may occur in the script for a reason beyond your control. In such cases, it is particularly important to write error-handling code.

#### A DEBUGGING WORKFLOW
###### Debugging is about deduction: eliminating potential causes of an error.
+ **WHERE IS THE PROBLEM?**:
1. Look at the error message.
2. Check how far the script is running.
3. Use breakpoints where things are going wrong.

+ **WHAT EXACTLY IS THE PROBLEM?**: 
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to.
2. Break down I break out parts of the code to test smaller pieces of the functionality.
3. Check the number of parameters for a function, or the number of items in an array.
