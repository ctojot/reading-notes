# Application State with Redux

## Dan Abramov Redux Tutorials

### What is the first principle of Redux?

The first principle of Redux is that everything that changes in your app, including the data and the UI state, is contained in a single object that we call the state or the state tree.

### What is a store and what do we use our reducers for within that store?

A store is basically a Javascript Object that holds the applications state and lets you dispatch actions. We use reducers to specify how the state should change in response to actions

### Name three Redux store methods given to us by createStore and describe their use.

- getState(): retireves the current state of the redux store
- dispatch(): lets you dispatch actions to change the state of your app
- subscribe(): lets you register a callback that the redux store will call anytime an action has dispatched

### Explain to a non-technical recruiter what combineReducers() does and why it is useful.

combineReducers() is a way to manage the state of a complex application. It can change things from information, product data, and settings. It is useful because it simplifies the management of complex application state by organizing and delegating responsibility to smaller, individual reducers, promoting modularity, maintainability, and scalability.

## Additional Questions

### Looking ahead at this module’s course schedule, What do you look forward to learning?

I'm looking forward to learning React Native.

### What are your learning goals after reading and reviewing the class README?

My goal is to finally get running and working app by the end of the week, I seem to be able to get any of the REACT apps finished.

## Reference

- ChatGPT