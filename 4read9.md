# Review, Research, and Discussion
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## How does route prefixing work with an external routing module?

[modularizing routes](https://medium.com/@shairez/angular-routing-a-better-pattern-for-large-scale-apps-f2890c952a18)

It works the same as routes declared within the same file, just need to import the router from an exterior module

## When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?

The only difference is the parameter selected.  id will return the id, and name will select the name from the object.

## Explain how Express handles routing conflicts?

Throws a 404 error, If the parent and the child have conflicting param names, the child’s value take precedence.

## What are the ways that a browser can send “data” or request variables to an HTTP server
HTTP request methods: GET, PUT POST

# Vocabulary Terms
- **Routing** [express docs definition](https://expressjs.com/en/4x/api.html#router) A router object is an isolated instance of middleware and routes. You can think of it as a “mini-application,” capable only of performing middleware and routing functions. Every Express application has a built-in app router.
- **Route Prefixing** [stack overflow](https://stackoverflow.com/questions/29993660/how-to-set-default-path-route-prefix-in-express) the prefix used before a route, keeps routing DRY
- **Request “Body”** data returned by the client to an API
- **Request “Query”** An object containing a property for each query string parameter in the route.
- **Request “Params”** . This property is an object containing properties mapped to the named route "parameters". For example, if you have the route /user/:name, then the "name" property is available as req.params.name. This object defaults to {}.  Request params are included in the route url ex: api/v1/categories/**parameter**


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


