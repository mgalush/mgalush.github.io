# Call Stack

In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

A **call stack** is a mechanism in JavaScript that keeps track of what function is currently being run and what functions are called from within that function.  It uses a **Last In, First Out (LIFO)** principle.

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

* When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function
* Any functions that are called by that function are added to the call stack further up, and run where their calls are reached
* When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing
* If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error


TLDR: 
* JavaScript is single-threaded, meaning it can only do one thing at a time
* Code execution is synchronous
* A function invocation creates a stack frame that occupies a temporary memory
* It works as a LIFO — Last In, First Out data structure