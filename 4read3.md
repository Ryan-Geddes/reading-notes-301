# Review, Research, and Discussion
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## Name 3 advantages to Test Driven Development
[advantages and disadvantages of TDD](https://medium.com/@stevenpcurtis.sc/test-driven-development-tdd-the-advantages-and-disadvantages-5347899ead90)
### Advantages: 
Testing and refactoring are baked into the process, which by definition encourages rigor in the production of quality code.
Unit testing itself encourages modularity in a codebase, and TDD helps with producing well-tested code that has a high percentage of test coverage.
The TDD process should save time in maintenance, as defects should be easy to find and are found early in the development process (a fail fast method of production).

### Disadvantages: 
TDD can (and certainly in the early stages of a software project it does) take longer to code and some of the advantages are only seen in the maintenance portion of the software development process. Some managers want to see code written now, and take the later consequences of poor development processes when (and if) they come.

## In what case would you need to use beforeEach() or afterEach() in a test suite?
You would use these functions if you need to reset an input or variable in the test environment before running the next test suite.

## What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

[prototypes vs es6](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up)

A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.

## Name a use case for a static method
Static methods are useful because they do not require a class instance to be run.

## Write an example of a Higher Order function and describe the use case it solves

Higher-order functions allow us to abstract over actions, not just values. They come in several forms. For example, we can have functions that create new functions.

```
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```

And we can have functions that change other functions.

```
function noisy(f) {
  return (...args) => {
    console.log("calling with", args);
    let result = f(...args);
    console.log("called with", args, ", returned", result);
    return result;
  };
}
noisy(Math.min)(3, 2, 1);
// → calling with [3, 2, 1]
// → called with [3, 2, 1] , returned 1
```

We can even write functions that provide new types of control flow.

```
function unless(test, then) {
  if (!test) then();
}

repeat(3, n => {
  unless(n % 2 == 1, () => {
    console.log(n, "is even");
  });
});
// → 0 is even
// → 2 is even
```



# Vocabulary Terms

- **functional programming**
- **pure function**
- **higher-order function**: Functions that operate on other functions, either by taking them as arguments or by returning them
- **immutable state**
- **object**
- **object-oriented programming (OOP)**: OOP stands for Object-Oriented Programming.

Procedural programming is about writing procedures or functions that perform operations on the data, while object-oriented programming is about creating objects that contain both data and functions.

Object-oriented programming has several advantages over procedural programming:

OOP is faster and easier to execute
OOP provides a clear structure for the programs
OOP helps to keep the C++ code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
OOP makes it possible to create full reusable applications with less code and shorter development time
- **class**
- **prototype**
- **super**
- **inheritance**
- **constructor**
- **instance**
- **context**
- **this** - refers to the object instance
- **Test Driven Development (TDD)**
- **Jest** - a testing library 
- **Continuous Integration (CI)**
- **unit test**



# Preview
	![alt text]('./Application Layer.jpg')

Which 3 things had you heard about previously and now have better clarity on?
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
What are you most excited about trying to implement or see how it works?

# Preparation Materials
[react hello world](https://facebook.github.io/react/docs/hello-world.html)
[introducing JSX](https://facebook.github.io/react/docs/introducing-jsx.html)
[rendering elements](https://facebook.github.io/react/docs/rendering-elements.html)



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


