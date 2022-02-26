# **El Reading Notes of the 401 Variety**

## **Class 32 reading notes**

### **El Questions**

1. **When you have multiple contexts, what component type should you use (class/function) and why?**
   - You can use either one, but using a function component would allow you to utilize the `useContext` hook.
   - [The Source](https://reactjs.org/docs/context.html) 
2. **What are some good use cases for using the Context API for global state?**
   - When some data needs to be accessible by many components at different nesting levels. 
   - [The Source](https://reactjs.org/docs/context.html) 
3. **How can you best test context?**
   - The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).
   - [The Source](https://www.samdawson.dev/article/react-context-testing)

### **Document the following Vocabulary Terms**

1. **context**
   - React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.
      - [The Source]()
2. **useContext()**
   - A hook used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.
      - [The Source]()
3. **static context**
   - A static method or, block belongs to the class and these will be loaded into the memory along with the class.

 <a href="#top">Take Me To The Repo!!</a>
