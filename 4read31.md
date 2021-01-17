# Hooks API

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## Why do we not need more .html pages in a multi-page React app?

React Routers allows you to put the content of a page inside a route component and switch to other pages that are contained inside a different route component

## If we wanted a component to show up on every page, where would we put it and why?

- Outside the ```<BrowserRouter/>```
- Inside the ```<BrowserRouter />```, outside a ```<Route />```
- Inside a ```<Route />```

The second option. To use routes, everything needs to be inside a BrowserRouter. For content to be seen by all pages, it can’t be inside a route component. The route component is meant for content that needs to be switched out if a user goes from page to page.

## What does props.children contain?
All child elements that are inside the components opening and closing tag.

# Vocabulary Terms
- **Children / Child Components** components nested inside other components
- **Hash Routing** uses URL hash, it puts no limitations on supported browsers or web server. Server-side routing is independent from client-side routing.
- **composition** the 'architecture' of the elements within a react page, assembling components as a collection of sub components



# Preparation Materials
[These are the concepts you should know in React.js (after you learn the basics)](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)
[ A quick intro to React’s props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
[Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
[React testing library api example](https://testing-library.com/docs/react-testing-library/example-intro/)



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


