# El Reading Notes of the 401 Variety

## Class 06 reading notes

### El Questions

#### Review, Research, and Discussion

##### Explain what a “Singleton” is (in Computer Science terms).

* In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.

[Source](https://en.wikipedia.org/wiki/Singleton_pattern#:~:text=In%20software%20engineering%2C%20the%20singleton,mathematical%20concept%20of%20a%20singleton.)

##### Explain how the Singleton pattern can be used with Node modules, specifically with classes.

* We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.

* The Singleton Pattern (an example for ya'll):

```js
class PrivateSingleton {
    constructor() {
        this.message = 'I am an instance';
    }
}
class Singleton {
    constructor() {
        throw new Error('Use Singleton.getInstance()');
    }
    static getInstance() {
        if (!Singleton.instance) {
            Singleton.instance = new PrivateSingleton();
        }
        return Singleton.instance;
    }
}
module.exports = Singleton;
```

* As we can see we actually created two classes `PrivateSingleton` and `Singleton`. This is a trick to hide (create pseudo-private) constructor in Singleton class.

* This way if we call `const object = new Singleton()` we will get an error: Use `Singleton.getInstance()`. However, if we call `Singleton.getInstance()` we will get the instance as expected. If there is no instance yet, we will call “private” constructor of `PrivateSingleton` class and return the instance. Otherwise, if the instance is already there, we simply return it.
We also export just `Singleton` so if we require it in another file, `PrivateSingleton` won’t be available.

[Source](https://medium.com/swlh/node-js-and-singleton-pattern-7b08d11c726a)

##### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

* First thing's first you have to install (or verify you installed) Node and NPM, which can be done by running this command in your terminal:

`npm -v && node -v`

* Then create a new project:

`npm init`

`npm install express --save`

* Copy and paste this code into your server.js file:

```js
const express = require('express');
const app = express();

app.get('/', (req, res, next) => {
  res.send('Welcome Home');
});

app.listen(3000);
```

* Then you'll wanna get that server up and running by running this code:

`node server.js`

[Source](https://developer.okta.com/blog/2018/09/13/build-and-understand-express-middleware-through-examples)

#### Document the following Vocabulary Terms

**Router Middleware**

> The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware.

[Source](https://stackoverflow.com/questions/63106648/what-is-router-middleware-in-express#:~:text=The%20term%20is%20composed%20of,or%20call%20the%20next%20middleware.)

**Dynamic Module Loading**

> Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

[Source](https://en.wikipedia.org/wiki/Dynamic_loading#:~:text=Dynamic%20loading%20is%20a%20mechanism,unload%20the%20library%20from%20memory.)

**Singleton Pattern**

> Singleton pattern is one of the simplest design patterns in Java. This type of design pattern comes under creational pattern as this pattern provides one of the best ways to create an object.

> This pattern involves a single class which is responsible to create an object while making sure that only single object gets created. This class provides a way to access its only object which can be accessed directly without need to instantiate the object of the class.

[Source](https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm)

**CRUD -> REST Method Matches**

```js
Create = POST
Read = GET
Update = PUT or PATCH
Delete = DELETE
```

**Mock Testing**

> Mocking means creating a fake version of an external or internal service that can stand in for the real one, helping your tests run more quickly and more reliably. When your implementation interacts with an object's properties, rather than its function or behavior, a mock can be used.

[Source](https://circleci.com/blog/how-to-test-software-part-i-mocking-stubbing-and-contract-testing/#:~:text=What%20is%20mock%20testing%3F,a%20mock%20can%20be%20used.)

 <a href="#top">Take Me To The Code!!</a>
