# Component Composition
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources
Joe Pennock's notes are more detailed and eloquent than those I wrote and will be more useful for my future reference so I have included them here.

## Can a parent component access the state of a child component?
Yes, a parent component can access the state of a child component, but not directly. You can’t simply access child.state or something like that. Instead, what you can do is have a method in the parent component that is passed to the child component. This method will give the child component the ability to pass state back up to the parent component.

## What can be passed along in a prop variable?
Props can be anything. You can pass object, arrays and even functions. Props are essentially the properties passed into a component when you ‘instantiate’ that component, to use JS terminology. If a component is a class, when you render that component inside of App you are essentially creating a new instance of that class. And as we know from ES6 class, what properties the constructor of the class have are the props of the new instance of that class. The same principle applies to React class components.


## How can a child component “know” the state of another component?
Since state is something unique to each component, child components can’t directly know the state of other components. In fact, a child doen’t even know that is might have sibling components. Instead, the way a child can know the state of other components is through props. The parent gives child1 a method to update the state of the parent. Child1 does stuff, sends the state to the parent. The parent now does the same thing and sends the new state from child1 to a new component, child2. Since components can’t directly access the state of other components, you need to go pass the state up to the parent and then back to another child.

# Vocabulary Terms
- **component props**  Props are the properties of a component class that were passed in when the class was rendered, or ‘instantiated’.
- **component state** state localized within the context of a single component
- **application state** 'global' state of the entire application at the top level


# Preparation Materials
[These are the concepts you should know in React.js (after you learn the basics)](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)
[ A quick intro to React’s props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
[Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
[React testing library api example](https://testing-library.com/docs/react-testing-library/example-intro/)



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


