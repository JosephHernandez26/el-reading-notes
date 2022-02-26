# **El Reading Notes of the 401 Variety**

## **Class 29 reading notes**

### **El Questions**

1. **How can we ensure that an effect hook runs only once?**
   - `useEffect` takes a second parameter. This will ensure `useEffect` only runs once.
     - *Note from the docs:* If you use this optimization, make sure the array includes all values from the component scope (such as props and state) that change over time and that are used by the effect.
   - [The Source](https://www.google.com/search?q=How+can+we+ensure+that+an+effect+hook+runs+only+once%3F+&rlz=1C1CHZN_enUS962US962&sxsrf=APq-WBtxgyzUlhMDz6i9qDGJTyXpyNCAbw%3A1645080920415&ei=WPENYozhGJm_0PEPxpuC-A8&ved=0ahUKEwiM7Yz_k4b2AhWZHzQIHcaNAP8Q4dUDCA8&uact=5&oq=How+can+we+ensure+that+an+effect+hook+runs+only+once%3F+&gs_lcp=Cgdnd3Mtd2l6EANKBAhBGABKBAhGGABQAFgAYKoHaABwAXgAgAFwiAFwkgEDMC4xmAEAoAECoAEBwAEB&sclient=gws-wiz) 
2. **Can useState() update more than one state variable at the same time?**
   - Yes use `useState` and an object then put in the `key` `value` pairs.
3. **Is useState() synchronous?**
   - No, `useState` is the asynchronous homie.
   - 
### **Document the following Vocabulary Terms**

1. **State Hook**
   - A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.
      - [The Source](https://reactjs.org/docs/hooks-state.html)
2. **Component Lifecycle**
   - The component lifecycle represents the various stages of a component as it is it called, rendered on a page (mounted), updated, or removed from a page (unmounted).
      - [The Source](https://reactjs.org/docs/hooks-reference.html#usereducer)

 <a href="#top">Take Me To The Repo!!</a>
 