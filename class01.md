# Introduction to html and css:
### How the Web Works?
**When you visit a website, the web server
hosting that site could be anywhere in the
world. In order for you to find the location of
the web server, your browser will first connect
to a Domain Name System (DNS) server. The unique number that the
DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a
computer that is constantly connected to the web, and is set up especially to send web pages to users.**

# Structure:
## HTML pages are text documents.
+ **Elements**: HTML Uses Elements to Describe the Structure of Pages. There are several different elements. Each element has an opening tag and a closing tag. Tags act like containers. They tell you something about the information that lies between their opening and closing tags. <p>
+ **Attributes**: Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign. <p lang="en-us">

# Extra Markup:
+ You can add comments to your code between the
<!-- and --> markers.
+ The id and class attributes allow you to identify
particular elements.
+ The <div> and <span> elements allow you to group
block-level and inline elements together.
+ The <meta> tag allows you to supply all kinds of
information about your web page.
+ Escape Characters: There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.) Therefore, if you want these characters to appear on your page you need to use what are termed "escape" characters(also known as escape codes or entity references). When using escape characters, it is important to check the page in your browser to ensure that the correct symbol shows up. such as <, >, and ©.

# HTML5 Layout:
#### HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them.
![image](https://www.homeandlearn.co.uk/WD/images/chapter6/one-col-layout-code.gif)

# Process & Design:
#### Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is. 
* ##### Know your target audience and understand their needs.
  + Ask questions about the people *who* that would be interested in your website.
    1. Target audience: Indivduals. 
    2. Target audience: Companies.

  + Know the reason *why* people would visit your website.
    1. Key Motivations: Are they looking for general entertainment or do they need to achieve a specific goal?
    2. Specific Goals: Do they want general information / researc (such as background on a topic /company), or are they after something specific (such as a particular fact or information on a product)?
* ##### Work out what information your audience need in order to achieve their goals quickly and effectively. By ensuring that you provide the information that your visitors are looking for, they will consider your site more relevant to them. Therefore, you will have more opportunity to tell them any extra information that you think would be helpful to them (or to expose them to other products and services you want to promote).
* ##### Do a *wireframe* for your website at first.A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.
* ### Start designing your website.
+ **Site Maps**: The aim is to create a diagram of the pages that will be used to structure the site. This is known as a site map and it will show how those pages can be grouped.
![image](https://i.pinimg.com/originals/1c/c5/f4/1cc5f4ec000969f11eedf4dbe0f8c9d8.png)
+ **WireFrames**: A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.
![image](https://miro.medium.com/max/900/0*FVLOt7Tx7P3zPI7T.jpg)

# Introduction to Java Script:
#### Javascript allows you to make web pages more interactive by accessing and modifying the content and markup used in a web page while it's being viewed in the browser.
+ **Access the content of the page**.
+ **Modify the content of the page**.
+ **Program rules or instructions the browser can follow**.
+ **React to events triggered by the user or browser**.

# The ABC of Programming:
#### A: What is a script and how do I creat one?
  A script is a series of instructions that acomputer can follow to achieve a goal. To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.
  + DEFINE THE GOAL
  + DESIGN THE SCRIPT: To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle.
  + CODE EACH STEP.
#### B: How do computers fit in the world around them?
 COMPUTERS CREATE MODELS OF THE WORLD USING DATA.
 + OBJECTS (THINGS):In computer programming, each physica l thing in
the world can be represented as an object.
+ PROPERTIES (CHARACTERISTICS): Each property has a name and a value, and each of these name/value pairs tells you something about each individual instance of the object.
+ EVENTS: Programs are designed to do different things when users interact with the computer in different ways. For example, clicking on a contact link on a web page could bring up a contact form.
+ METHODS: The code for a method can contain lots of instructions that together represent one task.
**Computers use data to create models of things in the real world.
The events, methods, and properties of an object all relate to each other: Events can trigger methods, and methods can retrieve or update an object's properties.**

  + **HOW A BROWSER SEES A WEB PAGE?**
  1. 1: The browser receive A PAGE AS HTML CODE.
  2. CREATE A MODEL OF THE PAGE AND STORE IT IN MEMORY.
  3. USE A RENDERING ENGINE TO SHOW THE PAGE ON SCREEN

#### C: How do I write a script for a web page?
JavaScript is written in plain text, just like HTML and CSS, so you do not need any new tools to write a script. When you want to use JavaScript with a web page, you use the HTML <script> element to tell the browser it is coming across a script. Its src attribute tells people where the JavaScript file is stored.
+ **PLACING THE SCRIPT IN THE PAGE**: You may see JavaScript in the HTML between opening <script> and closing </script> tags (but it is better to put scripts in their own files).
+ **JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML**: When the browser comes across a (script) element, it stops to load the script and then checks to see if it needs to do anything. The HTML (script) element is used to load the JavaScript file into the page. It has an attribute called src, whose value is the path to the script you created.
You may see JavaScript in the HTML between opening (script) and closing (/script) tags (but it is better to put scripts in their own files).
![image](https://miro.medium.com/max/2764/1*TeJb3sBvoF6tasJwDIbX8A.png)
