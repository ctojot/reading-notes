# Context API - Behaviors

## Scaling Up with Reducer and Context

### How do useReducer and useContext work together to simplify state management in a React application?

Reducers let you consolidtate a components state update logic. Context lets you pass informaton deep down to other components. Combining the two make state management a lot easier. With the reduce you can keep even handlers clear and concise but as an app grows, it becomes much more tedious when you have to pass the state down within the props. To counteract it, you would use context.

As stated before context lets you pass information into other components. Which means you can pass state to other components with context versus having to pass them down through the file heiracrchy. Any component can read and update the state as long as the state is above it in the heirarchy.

## Reference

- ChatGPT
