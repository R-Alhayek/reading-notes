# React Docs - thinking in React
![image](https://i.morioh.com/201022/2f6459ee.webp)

1. **How would you break a mock into a component heirarchy?**
+ The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. 
+ Use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. 
+ Separate your UI into components, where each component matches one piece of your data model.
+ You’ll see here that we have five components in our app. We’ve italicized the data each component represents:
           1. **FilterableProductTable (orange)**: contains the entirety of the example
           2. **SearchBar (blue)**: receives all user input
           3. **ProductTable (green)**: displays and filters the data collection based on user input
           4. **ProductCategoryRow (turquoise)**: displays a heading for each category
           5. **ProductRow (red)**: displays a row for each product.
.
2. **What is the single responsibility principle and how does it apply to components?**
 The **single responsibility principle**, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.
.
3. **What does it mean to build a ‘static’ version of your application?**
**‘static’ version of your application**: to build a version that takes your data model and renders the UI but has no interactivity. building a static version requires a lot of typing and no thinking. To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.
.
4. **Once you have a static application, what do you need to add?**
We need to add components that reuse other components and pass data using props. 
.
5. **What are the three questions you can ask to determine if something is state?**
   1. Is it passed in from a parent via props? If so, it probably isn’t state.
   2. Does it remain unchanged over time? If so, it probably isn’t state.
   3. Can you compute it based on any other state or props in your component? If so, it isn’t state.
.
6. **How can you identify where state needs to live?**
For each piece of state in your application:
+ Identify every component that renders something based on that state.
+ Find a common owner component (a single component above all the components that need the state in the hierarchy).
+ Either the common owner or another component higher up in the hierarchy should own the state.
+ If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

![image](https://cdn.sanity.io/images/xs6ohj1p/production/e7158d68d61834327067fed24c27fc3b43dfb222-1083x656.png?w=1200&fit=crop&auto=format)


## Things I want to know more about
