# useState() Hook

## Thinking in React

### Summarize the five steps of thinking in react

- Breaking the UI into a component heirarchy: its basically feels similar to how we whiteboard. First you start with the programming, deciding if you want to either create objects or functions. Then you would look at the CSS, specifically the class selectors. Lastly you focus on the design.

- Build a static version in React: start bulding the app, exluding any interaction. You want to render from the UI from the data model

- Find the minimal but complete representation of UI state: this is where the you need to figure out the minimum state the app needs and where it should be located

- Identify Where Your State Should Live: identify which part of the code should own the state.

- Add Inverse Data Flow: here you would give Children components ability to change the state of the parent components

## State: A Component’s Memory

### What is one reason a local variable isn’t sufficient for managing a React component?

Local variables do not trigger re-renders

### What is the argument to the useState hook, and what are the two parts of its return array?

The argument to the useState hook is the intial state value and the two parts of its return array are the state value and the function to set the state value.

### How can Component A access state from Component B?

Component A can access state from Component B through props if Component A is a child of Component B.