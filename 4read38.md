#  Redux - Asynchronous Actions

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## How granular should your reducers be?
Each reducer should control one aspect of state

## Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
There are both pros and cons of this. If you have intentions of having an action trigger two reducers, this can be beneficial. This can also be a con, if you accidently have two reducers that use the same action unintentionally.

## Name a strategy for preventing the above
Make sure your reducers are not responding to the same action.

# Vocabulary Terms

- **store** a store contains the whole state of your application
- **combined reducers** you must combine your reducers before exporting them to the store.  combines all the child reducers into one object and namespaces the state of each reducer under their own keys



# Preparation Materials
<h3 id="links">Links:</h3>

<ul>
  <li><a href="">dan abramov on suspense</a></li>
  <li><a href="https://redux.js.org/advanced/asyncactions">async actions</a></li>
  <li><a href="https://github.com/reduxjs/redux-thunk">thunk middleware</a></li>
  <li><a href="https://alligator.io/redux/redux-thunk/">redux thunk</a></li>
</ul>



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


