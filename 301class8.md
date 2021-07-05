# API Design Best Practices
![image](https://airspaceusa.com/wp-content/uploads/2016/10/api-icon.png)
1. **What does REST stand for?**
**REST**: Representational State Transfer.
.
2. **REST APIs are designed around a ____.**
REST APIs are designed around *resources*, which are any kind of object, data, or service that can be accessed by the client.
.
3. **What is an identifer of a resource? Give an example.**
*identifer* is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:HTTP.
.
4. **What are the most common HTTP verbs?**
The most common operations are GET, POST, PUT, PATCH, and DELETE.
.
5. **What should the URIs be based on?**
Resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
.
6. **Give an example of a good URI.**
It's a good practice to organize URIs for collections and items into a hierarchy. For example, /customers is the path to the customers collection, and /customers/5 is the path to the customer with ID equal to 5. This approach helps to keep the web API intuitive. Also, many web API frameworks can route requests based on parameterized URI paths, so you could define a route for the path /customers/{id}.
.
7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**
**"chatty"** web APIs expose a large number of small resources which is a bad thing because the more requests, the bigger the load.
.
8. **What status code does a successful GET request return?**
A successful GET method typically returns HTTP status code 200 (OK).
.
9. **What status code does an unsuccessful GET request return?**
If the resource cannot be found, the method should return 404 (Not Found).
.
10. **What status code does a successful POST request return?**
If a POST method creates a new resource, it returns HTTP status code 201 (Created).
If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body.
.
11. **What status code does a successful DELETE request return?**
If the delete operation is successful, the web server should respond with HTTP status code 204, indicating that the process has been successfully handled, but that the response body contains no further information. 

![image](https://miro.medium.com/max/1200/1*xJEUm1hUvxppvcjY14IKQA.jpeg)



## Things I want to know more about