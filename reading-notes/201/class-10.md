# Error Handling & Debugging

The JavaScript interpreter processes one line of code at a time.  When a statement needs data from another function, it stacks (or piles) the new function on top of the current stack

It uses the concept of **execution contexts**.  There is one global execution context and each function creates a new execution context

Every statement lives in one of three execution contexts:
1. **Global context**: code that is in the script, but not in a function
2. **Function context**: code that is being run within a function
3. **Eval context**: text that is executed like code in an internal function called eval()

Each time script enters a new execution context, there are two phases of activity:
#### Prepare: 
- A new scope is created
- Variables, functions, and arguments are created
- The value of the keyword `this` is determined

#### Execute
- Now it can assign values to variables
- Reference functions and their code
- Execute statements 

This is the basis of **hoisting** where variables and functions are created before they are executed and *hoisted* to the top of the execution statement

Functions in JavaScript are said to have **lexical scope**, meaning they are linked to the object they are defined within

When JavaScript generates an error, it throws an **exception**.  At that point, it stops and looks for execution-handling code.  If there is no exeuction-handling code, it stops and creates an **error object**

**Error Objects** can help you find where your mistakes are. When an error object is created, it will contain the following properties:
- name: type of execution
- message: description
- fileNumber: name of the javascript file
- lineNumber: line of the error

There are seven types of build-in error objects:
- error: generic error message
- syntax: syntax has not been followed
- ReferenceError: tried to reference a variable that is not defined
- TypeError: an unexpected data type
- RangeError: numbers not in an acceptable range
- URIError: encodeURI, decodeURI and similar methods not use appropriately
- EvalError: eval() funtion not used correctly

## How to deal with errors:
When debugging, try to narrow down the problem, eliminating potential causes of error.

1. debug the script: debug the code and trace the source of the error
2. handle errors gracefully: using `try`, `catch`, `throw`, and `finally` statements

```
try {
  // Try to execute this code
catch (exception) {
  // If there is an exception, run this code
finally {
  // This always gets executed
}
```

## `try`

First, specify the code you think might throw an exception within the `try` block

## `catch`
If `try` throws an exception, use `catch` for an alternative set of code

## `finally`
The code block `finally` will run either way and is used to clean up after the previous two clauses
