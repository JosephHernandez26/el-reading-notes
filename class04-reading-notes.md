# El Reading Notes of the 401 Variety

## Class 04 reading notes

### El Questions

#### Review, Research, and Discussion

##### 1. Name 3 advantages to Test Driven Development

1. Code is easier to maintain and more coherent.

2. Only the code necessary to pass the test is needed. Which is nice.

3. Makes development easier and more modularized.

[Source](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)

##### 2. In what case would you need to use beforeEach() or afterEach() in a test suite?

*  If each test in your describe needs a new copy of the structure because each test is modifying the structure then you should use `beforeEach` to create the structure anew for each test and then `afterEach` if you need to tear it down cleanly.
  * Doing this ensures test isolation: each test starts from a known state and does not depend on the presence or absence of a previous test to succeed.

[Source](https://stackoverflow.com/questions/21418580/what-is-the-difference-between-before-and-beforeeach)

##### 3. What is one downside of Test Driven Development

**No silver bullet** –
Tests help to seek out bugs, but they can not find bugs that you simply introduce within the test code and in implementation code. If you haven’t understood the matter you would like to unravel, writing tests most likely doesn’t help.
**slow process** –
If you begin TDD, you’ll get the sensation that you simply need an extended duration of your time for straightforward implementations. you would like to believe the interfaces, write the test code, and run the tests before you’ll finally start writing the code.
**All the members of a team got to do it** –
As TDD influences the planning of code, it’s recommended that either all the members of a team use TDD or nobody in the least. additionally, to the present, it’s sometimes difficult to justify TDD to the management because they often have the sensation that the implementation of latest features takes longer if developers write code that will not find themselves within the product half the time. It helps if the entire team agrees on the importance of unit tests.
**Tests got to be maintained when requirements change** –
Probably, the strongest argument against TDD is that the tests need to be maintained because the code has got to. Whenever requirements change, you would like to vary the code and tests. But you’re working with TDD. this suggests that you simply got to change the tests first then make the tests pass. So, actually, this disadvantage is that the same as before when writing code that apparently takes an extended time.y takes a long time.

[Source](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)

##### 4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

* A class defines all of the properties that characterize a certain set of objects (considering methods and fields in Java, or members in C++, to be properties). A class is abstract rather than any particular member in a set of objects it describes. For example, the Employee class could represent the set of all employees.
* An instance, on the other hand, is the instantiation of a class; that is. For example, Victoria could be an instance of the Employee class, representing a particular individual as an employee. An instance has exactly the same properties of its parent class (no more, no less).

[Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Details_of_the_Object_Model)

##### 5. Why REST?

**1. `REST` is Easy to Understand and Implement**
`REST` is meant to work over `HTTP` (actually `HTTP` was influenced by `REST`). Therefore it makes use of `HTTP` verbs that most of us know, such as `GET`, `POST`, and `PUT`.
**2. `REST` Makes your Application More Scalable**
There are 2 main reasons why `REST` can help make your application more scalable:
* **No State**
As we will see in the next section (Principles of `REST`), one of the core principles of `REST` is that it's stateless on the server-side. Therefore each request will be processed independently from the previous ones.
* **Faster Data Interchange Format*
RESTful APIs typically use `JSON` as the data interchange format. `JSON` is much more compact and smaller in size compared to XML. It can also be parsed faster than `XML`.

[Source](https://www.freecodecamp.org/news/benefits-of-rest/)

#### Document the following Vocabulary Terms

**functional programming**

>The process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.

[Source](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)

**Object-Oriented Programming (OOP)**

>Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

[Source](https://searchapparchitecture.techtarget.com/definition/object-oriented-programming-OOP)

**Class**

> Class is a blueprint for creating objects. A class encapsulates data and functions that manipulate data.

[Source](https://www.javascripttutorial.net/es6/javascript-class/#:~:text=A%20JavaScript%20class%20is%20a,classes%20are%20just%20special%20functions.)

**Super**

> The super keyword is used to access and call functions on an object's parent.

[Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super)

**This**

> It has different values depending on where it is used:

* In a method, this refers to the owner object.
* Alone, this refers to the global object.
* In a function, this refers to the global object.
* In a function, in strict mode, this is undefined.
* In an event, this refers to the element that received the event.
* Methods like `call()`, and `apply()` can refer this to any object.

[Source](https://www.w3schools.com/js/js_this.asp)

**Test Driven Development (TDD)**

> Test Driven Development (TDD) is a software development practice that focuses on creating unit test cases before developing the actual code. It is an iterative approach that combines programming, the creation of unit tests, and refactoring.

[Source](https://www.browserstack.com/guide/what-is-test-driven-development)

**Jest**

> Jest is a delightful JavaScript Testing Framework with a focus on simplicity.It works with projects using: Babel, TypeScript, Node, React, Angular, Vue and more!

[Source](https://jestjs.io/)

**Continuous Integration (CI)**

> Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early.

[Source](https://djangoshelton.medium.com/ci-cd-pipeline-patterns-for-javascript-part-1-df93f6a07dc8#:~:text=%E2%80%9CContinuous%20Integration%20(CI)%20is,to%20detect%20problems%20early.%20%E2%80%9C%20%E2%80%94)

**REST**

> Rest parameter is an improved way to handle function parameter, allowing us to more easily handle various input as parameters in a function.

[Source](https://www.geeksforgeeks.org/javascript-rest-operator/)

**Data Model**

> A data model (or datamodel)[1][2][3][4][5] is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. For instance, a data model may specify that the data element representing a car be composed of a number of other elements which, in turn, represent the color and size of the car and define its owner.

[Source](https://en.wikipedia.org/wiki/Data_model)

 <a href="#top">Take Me To The Top!!</a>
 