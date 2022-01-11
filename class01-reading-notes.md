# El Reading Notes of the 401 Variety

## Class 01 reading notes

### El Questions 

1. **Describe (in plain English) what Array.map() does**

* The Array.map() method allows you to iterate over an array and modify its elements using a callback function. The callback function will then be executed on each of the array's elements.
  * basically instead of iterating over an array using a loop, you can use this handy dandy method.
  * one thing of note...this method creates a **new** array.
  
* Code example:

```js
let arr = [2, 3, 5, 7]

arr.map(function(element, index, array){
	console.log(this) // 80
}, 80);
```

* [Source](https://www.freecodecamp.org/news/javascript-map-how-to-use-the-js-map-function-array-method/)

2. **Describe (in plain English) what Array.reduce() does**

* `Array.reduce()` iterates over the array and invokes the callback on each element. The difference is that instead of returning an array of equal size containing whatever was returned by the callback in each element, it returns whatever the final invocation of the callback returns.
* This is useful because, in addition to the current element and the index, the callback takes in the value that was returned by the previous invocation of the callback. MDN describes this as the “accumulator” because in most cases you will be modifying this value in some meaningful way and returning it for the next iteration to use.
* The reduce function takes as a second argument an initial value to use for the first iteration.
* A Coding example:

```js
let arr = [1, 2, 3, 4, 5]
let sum = arr.reduce((prev, cur) => prev + cur, 0)
console.log(sum) // 15
```

* [Source](https://javascript.plainenglish.io/what-is-array-reduce-4409d9706f27)

3. **Provide code snippets showing how to use superagent() to fetch data from a URL and log the result**

* Snippet example:

```js
request
   .post('/api/pet')
   .send({ name: 'Jack Skellington', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
  ```

* [Source](https://visionmedia.github.io/superagent/)

4. **With normal Promise .then() syntax**

```js
request
   .get('https://example.com/search')
   .then(res => {
   });
```
*[Source](https://visionmedia.github.io/superagent/)

5. **Again with async / await syntax**

```js
    async function doSomething() {
        try {
            const res = await callSuperagent();
            console.log('res', res);
            console.log('and our friend:', res.resImpVariable);
        } catch (error) {
            throw new Error(`Problem doing something: ${error}.`);
        }
    }

    doSomething();
```

* [Source](https://stackoverflow.com/questions/62187645/how-do-i-use-aysnc-await-in-this-superagent-call)

6. **Explain promises as though you were mentoring a Code 301 level student**

* A promise is an object that may produce a single value some time in the future: either a resolved value, or a reason that it’s not resolved (e.g., a network error occurred).

  **A promise is in one of three possible states:**
  * fulfilled (this step is completed)
  * rejected (an error occurred)
  * pending (this step  is in the queue to be completed)

7. **Are all callback functions considered to be Asynchronous? Why or Why Not?**

* The function that takes another function as an argument is called a higher-order function. According to this definition, any function can become a callback function if it is passed as an argument. Callbacks are not asynchronous by nature, but can be used for asynchronous purposes.
* Code example:

```js
// A function
function fn() {
  console.log('Just a function')
}
// A function that takes another function as an argument
function higherOrderFunction(callback) {
  // When you call a function that is passed as an argument, it is referred to as a callback
  callback()
}
// Passing a function
higherOrderFunction(fn)

// Output
// Just a function
```

* [Source](https://www.digitalocean.com/community/tutorials/understanding-the-event-loop-callbacks-promises-and-async-await-in-javascript)
