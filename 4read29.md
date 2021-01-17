# Routing
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources
Joe Pennock's notes are more detailed and eloquent than those I wrote and will be more useful for my future reference so I have included them here.

## Do child components have direct access to props/state from the parent?
Only if they have been explicitly passed down from the parent element via props.


As Joe says:


Child components do not have direct access to the props or state of the parent component. In order for the child component to read or update the state of the parent, the child either needs to be passed a method for accessing the state from the parent or have the parent’s state passed in as props to the child. The former will allow the child to update the state of the parent component. The latter will just give the child component read access.


## When a component “wraps” another component, how does the child component’s output get rendered?

```
<Main>
  <Content />
</Main>
```
The markup within 'content' will be rendered as if it was written within the 'main' component.

## Can a component, such as ```<Content />```, which is a child also be used as a standalone component elsewhere in the application?

Yes, if it is exported from a module and imported into the file.

From Joe:

All components in React can be considered standalone components. Thus, any child component that was created and rendered in a parent component can also be imported and used elsewhere. The only consideration would need to be if the child component has props from the parent required to make it work. But ideally, all components should be created in such a way that they can be reused anywhere in an application that makes sense.

## What trick can a parent use to share all props with it’s children

Inside of the render of the parent component, you can simply send props.children to the child component. Props.children are whatever is inside the JSX tags when rendering out a component.

# Vocabulary Terms
- **props.children**  these are used to display whatever is put inside if the opening/closing tags of a component when rendering it.
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


