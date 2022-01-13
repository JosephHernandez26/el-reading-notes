# El Reading Notes of the 401 Variety

## Class 03 reading notes

### El Questions 

1. **Name 3 real world use cases where you’d want to change the request with custom middleware**

* Password checking before sending the client information on their account

  * Sensitive information being collected

    * Verification of available information on records

2. **True or false: The route handler is middleware?**

* **F A L S E**

3. **In what ways can a middleware function end the process and send data to the browser?**

* Through the invocation of the `next()` function.

  * If invalid information is passed the `res.status(404)` error can be thrown to end the process.

4. **At what point in the request lifecycle can you “inject” middleware?**

* Basically as soon as the request reaches the server.

5. **What can cause express to error with “Request headers sent twice, cannot start a second response”**

* This happens when the server sends two responses, typically within a route handler. Once `res.send()` has been called, it cannot be called a second time.

### Document the following Vocabulary Terms

#### Term

**Middleware**

> Middleware is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

[Source](https://azure.microsoft.com/en-us/overview/what-is-middleware/)

**Request Object**

> The request object is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. Examples of requests passed to the Library are a client application issuing a GET request on a HTTP URL, or a server issuing a load on a local file URL.

[Source](https://www.w3.org/Library/User/Using/Request.html#:~:text=The%20request%20object%20is%20the,must%20use%20a%20Request%20object.&text=Examples%20of%20requests%20passed%20to,on%20a%20local%20file%20URL.)

**Response Object**

> The Response interface of the Fetch API represents the response to a request.

[Source](https://developer.mozilla.org/en-US/docs/Web/API/Response)

**Application Middleware**

> Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. 

[Source](https://expressjs.com/en/guide/writing-middleware.html)

**Routing Middleware**

> Middlewares are features added on top of his basic handler, in the form of a stack of functions that take this request into a pipeline doing stuff with it (logging, parsing body, security ...ect).

[Source](https://stackoverflow.com/questions/63106648/what-is-router-middleware-in-express)

**Test Driven Development**

> Test-driven development is the act of first deciding what you want your program to do (the specifications), formulating a failing test, then writing the code to make that test pass. It is most often associated with automated testing. Although you could apply the principals to manual testing as well.

[Source](https://www.freecodecamp.org/news/an-introduction-to-test-driven-development-c4de6dce5c/)

**Behavioral Testing**

> Is a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests.

[Source](https://medium.com/javascript-scene/behavior-driven-development-bdd-and-functional-testing-62084ad7f1f2)

[Take Me To The Top, NOW!](#)
