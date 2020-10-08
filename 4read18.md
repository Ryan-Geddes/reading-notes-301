# Review, Research, and Discussion
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

## Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
Calling a server route is a backened event, as is an event emitter.

## Why are events sometimes better than asynchronous actions with callbacks?
(https://stackoverflow.com/questions/2069763/difference-between-event-handlers-and-callbacks#:~:text=Usually%20the%20myaction%20program%20will,for%20a%20more%20responsive%20GUI.&text=A%20callback%20is%20procedure%20you%20pass%20as%20an%20argument%20to%20another%20procedure.)
Generally speaking, a 'callback' is under the control of the detecting process. So you tell a GUI manager "call myaction when this button is pressed" and the GUI manager calls the action when the button is pressed.

Event Handlers on the other hand operate at one step removed. The GUI manager is configured to send messages to an event handler. You tell an event manager that button pushes are handled by the myaction program. When the button is pushed the GUI manager puts a message on the event handler's queue and gets on with GUI managing. The event handler picks up the message from the queue, sees it's a button push, fires up the myaction program, and moves on to handling the next event. Usually the myaction program will run as an independent thread or even a separate process.

While the "event handler" pattern is more complex it is much more robust and less likely to hang when an action fails. It also makes for a more responsive GUI.

## What does an EventEmitter instance do?
From the reading:

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter. on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

## When is a program’s call stack, event queue, and event loop active?
The call stack is active whenever the program is ran, and runs sequentially through each function.  The event queue is a list of async callback functions that are looped whenever the callstack is empty.

# Vocabulary Terms
- **OSI** - Open System Interconnection
- **Observer Pattern** - The observer pattern is a software design pattern in which an object, called the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. It is mainly used to implement distributed event handling systems.
- **Listener** - this is the function that is invokes a callback when the specific event is detected
- **Event Handler** - a callback function called when an event is triggerd
- **Event Driven Programming** - event-driven programming is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or messages from other programs or threads. 
- **Event Loop** - the loop of functions run through the call stack and queue
- **Event Queue** - This is a queue of callback functions that are run only when the call stack is empty
- **Call Stack** - The call stack is the primary order that functions are ran in JS
- **Emit/Raise/Trigger** - This is the name for the trigger for an event 
- **Subscribe** - publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are.


# Preview
	![alt text]('./Application Layer.jpg')

Which 3 things had you heard about previously and now have better clarity on?
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
What are you most excited about trying to implement or see how it works?

# Preparation Materials
[What is the event Loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
[Node events](https://nodejs.org/api/events.html)
[Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)



How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.


