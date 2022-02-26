# **El Reading Notes of the 401 Variety**

## **Class 28 reading notes**

### **El Questions**

1. **Why do we not need more .html pages in a multi-page React app?**
   - React is a single page application which requires a root in an HTML page.
   - If your project requires multiple webpages you will need multiple HTML pages which means multiple roots can be set up.
2. **If we wanted a component to show up on every page, where would we put it and why?**
   - *Outside* `<BrowserRouter/>`
   - *Inside* `<BrowserRouter />`
   - *Outside* a `<Route />` and *Inside* a `<Route />`.
3. **What does routing do with the components that were rendered when a new route is requested?**
   - If the component isn't required to render at the new route, the render function isn't called.
4. **What does `props.children` contain?**
   - `props.children` contains any State attributes or Function attributes passed down from a parent component to a child component.
5. **How do `useState()` and `this.setState()` differ?**
   - `useSate()` is a *hook* from the **ReactAPI** and can only be used with functional components
   - `this.setState()` is used with class based components.

### **Document the following Vocabulary Terms**

1. **State Hook**
   - A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.
      - [The Source](https://reactjs.org/docs/hooks-state.html)
2. **Mounting and Un-Mounting**
   - A React component’s lifecycle contains distinct phases for creation and deletion. In coding terms, these are called mounting and unmounting. You can also think of them as “setup” and “cleanup”.
      - [The Source](https://learn.co/lessons/react-component-mounting-and-unmounting)

 <a href="#top">Take Me To The Repo!!</a>
