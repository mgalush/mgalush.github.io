# Functional Programming

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

## Pure functions

Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result.

A function is pure if:
* It returns the same result if given the same arguments

For example, imagine we have this function:
```
let PI = 3.14;

const calculateArea = (radius) => radius * radius * PI;

calculateArea(10); // returns 314.0
```
This function is not pure because it uses a global object that was not passed as a parameter to the function.  Therefore, if someone changed the global variable (`PI`), it would produce a different result.

If a function reads external files or generates random numbers, it is also not pure.

* It does not cause any observable side effects

Observable side effects could be modifying a global object or a passed parameter.

```
let counter = 1;

function increaseCounter(value) {
  counter = value + 1;
}

increaseCounter(counter);
console.log(counter); // 2
```
The code above is not pure, but by doing the following, you can make it pure:
```
let counter = 1;

const increaseCounter = (value) => value + 1;

increaseCounter(counter); // 2
console.log(counter); // 1
```

## Immutability 

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## Referential transparency

If a function consistently yields the same result for the same input, it is referentially transparent.

### pure functions + immutable data = referential transparency

The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

## Functions as first-class entities
Functions as first-class entities can:
* refer to it from constants and variables
* pass it as a parameter to other functions
* return it as result from other functions

## Higher order functions

A function that either:
* takes one or more functions as arguments, or
* returns a function as its result


# How to write clean code

* Return early from functions
* Cache variables so functions can be read like sentences
* Check for Web APIs before implementing your own functionality