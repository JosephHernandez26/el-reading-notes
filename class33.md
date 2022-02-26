# **El Reading Notes of the 401 Variety**

## **Class 33 reading notes**

### **El Questions**

1. **Why is the Context API useful?**
   - The Context API can be used to share data with multiple components, without having to pass data through props manually. For example, some use cases the Context API is ideal for:
     - Theming,
     - User language,
     - Authentication,
     - *among other things* 
   - [The Source](https://www.telerik.com/blogs/understand-react-context-api#:~:text=The%20Context%20API%20can%20be,user%20language%2C%20authentication%2C%20etc.)
2. **Can a component outside of a provider get its context?**
   - To access a React context outside of the render function, we can use the `useContext` hook.
   - We create the `UserContext` by calling the React `createContext` method with a default context value.
   - Then in the `Users` component, we call the `useContext` hook with `UserContext` to access the current value of `UserContext`.
   - [The Source](https://thewebdev.info/2021/05/28/how-to-access-a-react-context-outside-of-the-render-function/#:~:text=the%20render%20Function-,To%20access%20a%20React%20context%20outside%20of%20the%20render%20function,can%20use%20the%20useContext%20hook.&text=We%20create%20the%20UserContext%20by,the%20current%20value%20of%20UserContext%20.)
3. **What are some common use cases for using the Context API?**
   - User Settings,
   - Theme,
   - Autnentication
   - [The Source](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more) 
4. **Describe “Context Hell”**
   - React 'Context Hell' is the awful nasty code you get when taking advantage of the React Context API.
   - [The Source](https://dev.to/alfredosalzillo/the-react-context-hell-7p4)

### **Document the following Vocabulary Terms**

1. **Global State**
   - Global State is State in React and can be considered the State provided to Context.
      - [The Source](https://www.npmjs.com/package/react-cookies)
2. **Global Context**
   - global context is the context component that provides global state
      - [The Source](https://www.npmjs.com/package/react-cookies)
3. **Provider**
   - A context element that when wrapped around an element provides that element and it's children the ability to use context.
      - [The Source](https://www.npmjs.com/package/react-cookies)
4. **Consumer**
   - any element that uses the context passed through by a provider
      - [The Source](https://www.npmjs.com/package/react-cookies)

 <a href="#top">Take Me To The Repo!!</a>
