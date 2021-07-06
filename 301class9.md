# Functional Programming Concepts
![image](https://www.modernescpp.com/images/blog/Functional/PureFunctions/CharakteristikPureFunctionsEng.png)
1. **What is functional programming?**
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia
.
2. **What is a pure function and how do we know if something is a pure function?**
**pure function** returns the same result if given the same arguments (it is also referred as deterministic) and it does not cause any observable side effects.
.
3. **What are the benefits of a pure function?**
The code’s definitely easier to test. We don’t need to mock anything. 
.
4. **What is immutability?**
Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
.
5. **What is Referential transparency?**
A function that consistently yields the same result for the same input.

![image](https://cdn-images-1.medium.com/max/1600/0*a_yub2gTwY-1eK8j.png)

# Node JS Tutorial for Beginners #6 - Modules and require()
1. **What is a module?**
Other JAVA SCRIPT files that we split our code into. Each module has a little bit of code which has different functionality and we call them whenever we need them.
.
2. **What does the word ‘require’ do?**
A function used on the global js so we can use it wherever we want.
.
3. **How do we bring another module into the file the we are working in?**
We write **require** then ('./file-name') and inside them we have a string which is the path to the module that we require in this file.
**EX**: *require('./file-name')*
.
4. **What do we have to do to make a module available?**
Inside the module itself, we will present which part of the module we want to be available for all the files that requires it.
**module.export = What will be available outside this module and we set a variable to the require in the file we want the module in**

![image](https://cdn-media-1.freecodecamp.org/images/1*tZaoIiIYEv0bc0bLO-CYVg.png)



## Things I want to know more about