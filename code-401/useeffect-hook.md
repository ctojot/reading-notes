# Component Lifecycle / useEffect Hook

## useEffect hook

### What is the main intended use case for the useEffect hook?

The inteded use case for useEffect is only to call it at the top level of a component or custom hooks. It cannot be called inside loop or conditions.

### How does the effect’s logic interact with the component?

If you have dependencies that are objects or functions inside of a component, it might casue effect to re-run a number of times than necessary.

### What is the importance of the return value from the effect’s logic function?

The return value is an optional cleanup function.  React will first run the cleanup function with the old values, and then run your setup function with the new values. When the component is removed from the DOM, React will run your cleanup function,

### What are your learning goals after reading and reviewing the class README?

Still the same. State and props are still confusing so i need to get those straight.
