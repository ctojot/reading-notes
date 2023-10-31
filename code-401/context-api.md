# Context API

## Choosing the State Structure

### Summarize the five principles for structuring state.

- Group related state: Updating the state to a single state when you need to update 2 or more state variables at the same time.

- Avoid contradictions in state: Steer away from creating a state where several pieces of it can contradict and disagree with each other.

- Avoid redundant state: Calculating information for a components props during rendering and not putting that information into state.

- Avoid duplication in state: When the same data is duplicated between multiple state variables, or within nested objects.

- Avoid deeply nested state: When there is a deeply hierarchial state, making it inconvenient to update.

## Passing State Deeply with Context

### What problem do Contexts aim to solve?

Passing props can become verbose and inconvenient when you need to pass some prop deeply through a tree, or if many components need the same prop. Context lets a parent components provide data to the entire tree below it.

### What is one technique to try before useContext?

You can either start by passing props or Extract components and pass JSX as children to them.

### What hook complements useContext for complex applications?

useReducer is commonly used with context to manage complex state and pass it down to distant components without hassle.

## References

- ChatGPT