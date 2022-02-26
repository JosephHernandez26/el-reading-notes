# **El Reading Notes of the 401 Variety**

## **Class 31 reading notes**

### **El Questions**

1. **Describe use cases useState() vs useReducer()**
   - `useReducer` is usually preferable to `useState` when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
   - `useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.
   - [The Source](https://github.com/diegohaz/awesome-react-context) 
2. **Why do custom hooks need the use prefix?**
   - Custom Hooks should start with the `use` prefix so to make it clear the Hook's rules apply directly, which allows React to check for violations of those rules.
   - [The Source](https://github.com/diegohaz/awesome-react-context) 
3. **What do custom hooks usually do?**
   - Custom Hooks allow the removal of duplicated logic from two different Components requiring changes on the same State.
   - State is not shared between them, they are tools for the reuse of stateful logic.
   - [The Source](https://github.com/diegohaz/awesome-react-context) 
4. **Using any list of custom hooks, research and name one that you think will be useful in your applications**
   - `useToggle()` is a custom Hook and would be useful anytime incorporation or manipulation of State goes from `true` to `false` or `false` to `true`.
   - [The Source](https://github.com/diegohaz/awesome-react-context)
5. **Describe how a hook that fetches API data might work**
   - The Hook fetches API data by using Axios to query the API and store the response in State.
   - [The Source](https://github.com/diegohaz/awesome-react-context) 

### **Document the following Vocabulary Terms**

1. **Reducer**
   - A Reducer is a pure function that takes the current State and action,
     - And returns the new State result.
     - For example: `(state, action) => newState`
      - [The Source](https://usehooks.com/)

 <a href="#top">Take Me To The Repo!!</a>
