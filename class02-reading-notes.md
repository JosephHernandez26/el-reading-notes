# El Reading Notes of the 401 Variety

## Class 02 reading notes

### El Questions 

1. **What’s the difference between `PUT` and `PATCH`?**

* `PUT` is a method of modifying resources where the client sends data that updates the entire resource.
  * **Code**

  ```js
  let PutRequest = () => {
  // Sending PUT request with fetch API in javascript
  fetch("https://reqres.in/api/users/2", {
    headers: {
      Accept: "application/json",
      "Content-Type": "application/json"
    },
    method: "PUT",
 
    // Sending only the fields that to be updated
    body: JSON.stringify({      
      email: "hello@geeky.com",
      first_name: "Geeky"
    })
  })
    .then(function (response) {
 
      // Console.log(response);
      return response.json();
    })
    .then(function (data) {
      console.log(data);
    });
  
  });
  
  PutRequest();


* Unlike `PUT` Request, `PATCH` does partial update e.g. Fields that need to be updated by the client, only that field is updated without modifying the other field.
  * **Code**

```js

let PatchRequest = () => {
  // sending PUT request with fetch API in javascript
  fetch("https://reqres.in/api/users/2", {
    headers: {
      Accept: "application/json",
      "Content-Type": "application/json"
    },
    method: "PATCH",    
 
    // Fields that to be updated are passed
    body: JSON.stringify({
      email: "hello@geeky.com",
      first_name: "Geeky"
    })
  })
    .then(function (response) {
 
      // console.log(response);
      return response.json();
    })
    .then(function (data) {
      console.log(data);
    });
};
 
PatchRequest();
```

[Source](https://www.geeksforgeeks.org/difference-between-put-and-patch-request/)

2. **Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`**

[Mockoon](https://mockoon.com/)

[Mocky.io](https://designer.mocky.io/)

[Mock Server](https://www.mock-server.com/)

3. **Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?**

* Swagger & APIDoc.js are very similar in that they both require documentation implementation.
  * Swagger is much more popular and is a cloud based testing and documentation tool used by some of the most popular companies around. 
  
  [Swagger](https://swagger.io/solutions/api-documentation/)
  
  * APIDoc creates its documentation from API annotations in the source code, and is a lot less popular.
  
  [APIDocs.js](https://apidocjs.com/)
  
    * **HTTP Status UN-Successful Codes:**
    * Client error responses (400–499)
    * Server error responses (500–599)

4. **Compare and contrast `SOAP` and `ReST`**

* `SOAP` stands for **Simple Object Access Protocol**
  * `SOAP` is a protocol, it follows a strict standard to allow communication between the client and the server.
  * Uses only XML for exchanging information in its message format.
  * Is difficult to implement and it requires more bandwidth.
  * Benefits of `SOAP` over `REST` as `SOAP` has `ACID` compliance transaction.
* `REST` stands for **REpresentational State Transfer**
  * `REST` is an architectural style that doesn’t follow any strict standard but follows **six constraints** defined by Roy Fielding in 2000.
    * Uniform Interface,
    * Client-Server,
    * Stateless,
    * Cacheable,
    * Layered System,
    * Code on Demand.
  * Is not restricted to XML and its the choice of implementer which Media-Type to use like XML, JSON, Plain-text.
  * `REST` can use `SOAP` protocol but `SOAP` cannot use `REST`.
  * Is easy to implement and requires less bandwidth such as smartphones.
  * `REST` lacks in sufficient security protocols that `SOAP` excels in, it depends on your application requirement.

  [Source](https://www.geeksforgeeks.org/difference-between-rest-api-and-soap-api/)

### Document the following Vocabulary Terms

1. **Web Server**

>> A web server is software and hardware that uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the World Wide Web.

2. **Express**

>> Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

3. **Routing**

>> Routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route.

4. **WRRC**

>> Web request/response cycle.

### Preview

1. **Which 3 things had you heard about previously and now have better clarity on?**

* Honestly, what `Node.js` is for real. I mean, I knew what it was vaguely, now I have far more clarity on its actual uses and benefits than I did before.
  * What `SOAP` and `REST` are and their key differences/uses.
    * What Express is.

2. **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* I would like to see or hear a more detailed explanation around implementing the Express server and getting her to run smoothly.
  * `PUT` and `PATCH` and how to use these effectively.
    * The proper use of APIDocs.js and Swagger.

3. **What are you most excited about trying to implement or see how it works?**

* I mean, I am always stoked to see something I just learned implemented and running smoothly. So, I am here for all of that stuff.
