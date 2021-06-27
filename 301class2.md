# React lifecycle
![image](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
**‘render’** hapens first.

2. **What is the very first thing to happen in the lifecycle of React?**
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. So creating a **Constructo** is the first thing to happen.

3. **Put the following things in the order that they happen: *componentDidMount*, *render*, *constructor*, *componentWillUnmount*, *React Updates***.
    1.**constructor**
    2. **render**
    3. **componentDidMount**
    4. **React Updates**
    5. **componentWillUnmount**


4. **What does componentDidMount do?**
We use it when we need to load anything using a network request or initialize the DOM. This method is a good place to set up any subscriptions.



# React State Vs Props
1. **What types of things can you pass in the props?**
- The initial components of the **props**.
- Using **Props**, we can pass values from aparent components down to child components. This includes any data type, from strings to functions, objects, etc..

2. **What is the big difference between props and state?**
With **Props** you pass into a component and  **State** IS handled inside of that component, while **Props** are handled outside of the component.

3. **When do we re-render our application?**
We use **State** when we need to re-render and update the application based on something the user do.

4. **What are some examples of things that we could store in state?**
+ Data that the user update/enter inside a form
+ counters
...
![image](https://www.techdiagonal.com/wp-content/uploads/2019/09/react-props-blog-image-design-2.jpg)



## Things I want to know more about