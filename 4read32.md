# Custom Hooks

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## What does a component’s lifecycle refer to?

The three phases of a component's lifecycle:

- Mounting
- Updating
- Unmounting

Mounting - putting elements into the dom
Updating - whenever there is a change in the components state or prop
Unmounting - when a component is removed from the DOM

## Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
UseCallback helps you prevent infinite loops. Whenver a function is inside another function, it gets recreated whenever the outer function runs. When that innerfunction is a dependency of useEffect(), this creates an infinite loop. When a components rebuilds, the innerfunction changes, and the outer function reruns, creating an infinite loop.
## Why are functional components preferred over class components?

Functional components are cleaner and easier to follow.  Also can have individual states passed down instance of class instances
## What is wrong with the following code?

The for loop should be inside the use effect.


```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

# Vocabulary Terms
- **state hook** hook that lets you add React state to function component.
- **effect hook** allows you to register a function which executes after the current render cycle. perform side effects in function components
- **reducer hook** accepts a reducer function with the application initial state, returns the current application state, then dispatches a function.



# Preparation Materials
<h3 id="links">Links:</h3>

<ul>
  <li><a href="https://www.telerik.com/blogs/everything-you-need-to-create-a-custom-react-hook">custom hooks - all you need to know</a></li>
  <li><a href="https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g">async hooks</a></li>
  <li><a href="https://reactjs.org/docs/hooks-reference.html#usereducer">useReducer Hook</a></li>
  <li><a href="https://reactjs.org/docs/hooks-custom.html">react custom hooks</a></li>
  <li><a href="https://usehooks.com/">use hooks</a></li>
  <li><a href="https://github.com/rehooks/awesome-react-hooks">hooks list</a></li>
  <li><a href="https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d">10 essential react hooks</a></li>
</ul>



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


