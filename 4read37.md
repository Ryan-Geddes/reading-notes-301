# Context API

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## Describe use cases for useMemo() and useReducer()

useReducer() is preferred when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useMemo() will check if any dependencies have changed, if not, it will return the cached return value, not calling the function. It helps optimize performance.

## Why do custom hooks need the use prefix?

It's a react semantic naming convention.  I believe react treats useFunctions differently as well.

## What do custom hooks usually do?
You ususally write a custom hook to replace a app specific function that is being reused.

Custom Hooks are a mechanism to reuse stateful logic (such as setting up a subscription and remembering the current value), but every time you use a custom Hook, all state and effects inside of it are fully isolated.

## Using any list of custom hooks, research and name one that you think will be useful in your applications

## Describe how a hook that fetches API data might work
You can use useEffect() with async/await workarounds to fetch API data. The following are three known ways to make an API call utilizing useEffect():

Async method 1 is REACT recommended

```
useEffect(() => {
const search = async () => {
const { data } = await axios.get('https://en.wikipedia.org/w/api.php', {
  params: {
    action: 'query',
    list: 'search',
    origin: '*',
    format: 'json',
    srsearch: term
  }
});
setResults(data.query.search);
}
if (term) {
search();
}
}, [term]);
```

```
(async () => {
await
axios.get('stuff');
})();
```

```
axios.get('stuff')
.then((data) => {console.log(response.data)})
```

# Vocabulary Terms

- **reducer** [reducer definition](https://reactjs.org/docs/hooks-reference.html#usereducer) An alternative to useState()
Accepts a reducer type (state, action) => newState and returns the current state paired with a dispatch method.
useReducer is usually preferable to useState when you have comlex state logic that involves multi-sub-values or when the next state depends on the previous one.
also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks



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


