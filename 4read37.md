# Redux - Combined Reducers

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## Why choose Redux instead of the Context API for global state?

Context triggers a re-render every single time a state variable changes.  Redux only updates a slice of the state, just the part that changes.  Redux is better for applications with frequent updates and more complex states. Also changes to states are centralized and happen one by one in a strict order so there are no subtle race conditions to watch out for.

## What is the purpose of a reducer?
It will update the state depending on which action gets dispatched

## What does an action contain?
A type and a payload

## Why do we need to copy the state in a reducer?
Reducers are pure functions that take the previous state and action and return the next state. Reducers are never allowed to mutate the original/current state values. It must make “immutable updates” by copying the existing state and making changes to the copied values.
# Vocabulary Terms

- **immutable state** unchangeable state
- **time travel in redux** the ability to see dispatched actions and the state of the redux store at every point in time. This makes it possible to inspect the state and travel back in time to previous state without reloading the page or restarting the app. Use Redux DevTools
- **action creator** a function that returns an action object
- **reducer** these are functions with state and actions passed in. These work with action.type in switch cases and return the updated state it optionally needs to accept payload to work properly. Sometimes you will need to merge separate reducers before creating a store
- **dispatch** a method in redux that will use an action object to trigger the reducer to update a state
- **pure function** A pure function is a function which given the same input, will always return the same output and produces no side effects.  A dead giveaway that a function is impure is if it makes sense to call it without using its return value. For pure functions, that’s a noop.
[what is a pure function](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)



# Preparation Materials
<h3 id="links">Links:</h3>

<ul>
  <li><a href="https://www.youtube.com/watch?v=gBER4Or86hE">Multiple Reducers Example</a></li>
  <li><a href="https://redux.js.org/recipes/structuring-reducers/using-combinereducers/">Redux Docs: Using Combined Reducers</a></li>
  <li><a href="https://redux.js.org/api/combinereducers/">Redux Docs: Combined Reducer Syntax</a></li>
</ul>



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


