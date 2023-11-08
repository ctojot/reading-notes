# Redux - Asynchronous Actions

## async actions

### Why use Redux middleware?

Redux middleware is useful because it allows you to do things that you aren't normally able to. For example, a redux reducers aren't capable of having side effects. With middleware you enable the ability to write logic with sideffects.

### Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

The data flow starts when an action is dispatched. After the action is dispatched, a reducer is called and changes the state based on the current state and the action. The new state is then returned and the subscribers or the components of the app are listening for the state changes.

### How are we accommodating async in our Redux app?

By using middleware, specifically the redux thunk middleware. Thunk functions can have async logic within it.

## thunk middleware

### Why would you need redux-thunk middleware?

You would need redux-thunk whenever your redux app requires the use of async actions.

### Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

Function

### Describe how any return value from the inner thunk function will be made available.

Through the use of the dispatch and getState functions passed as arguments to the thunk function.

## Reflection

### What are your learning goals after reading and reviewing the class README?

Get better at writing logic for functions.
