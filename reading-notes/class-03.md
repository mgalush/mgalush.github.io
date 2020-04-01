# Decision Making in JavaScript
**Conditions** can help you determine which path to take when writing code. 

Two parts of a decision:
1.  An expression is evaluated
2.  A conditional statement says what to do in a given situation
```
    if (x > 50) {
    document.write('You passed!');
    } else {
    document.write('Try Again');
    }
```
### You can evaluate conditions using operators

Comparison operators: `==`, `!=`, `===`, `<`, `>`, `>=`, or `<=`.

Logical operators: `&&`, `||`, or `!`

# If Statements

## If statements
In an **if** statement, the condition evaluates to `true`, the code block is executed:
```
if (score >= 50) {
  congratulate();
}
```
## if... else statements

In an **if... else** statement, the condition is checked and only the code block that evaluates as `true` will run:

```
if (score >= 50) {
  congratulate();
} else {
  encourage();
}
```

## switch statements

In a **switch statement**, each case indicates a possible value for the variable and the code that matches the variable will run:

```
switch (level) {
  case 'one':
  title = 'level 1';
  break;

  case 'two':
  title = 'level 2';
  break;

  case 'three':
  title = 'level 3';
  break;

  default:
  title = 'test';
  break;
}
```


Note: all variables in an **if** or **if... else** statement are evaluated and checked even when a match has been found, whereas in the **switch** statement, the code breaks the statement and stops stops as soon as a match has been found.


# JavaScript Data Types

- String: text
- Number: number
- Boolean: true or false
- Null: empty value
- Undefined: variable has not been assigned

*NaN is a value that is counted as number*

**All numbers in JavaScript are treated as if they are true (truthy) or false (falsy).**

0 = falsy
1 = truthy

# JavaScript Loops

Loops check a condtion.  If it returns true, the code block will run, and continue to run, until it returns false.

There are three types of loops:
- for
- while
- do while 

### For loops

Use when you need to run code a specific number of times

### While loops

Use when you do not know how many times the code should run

### Do While loops

Use when you do not know how many times the code should run but you do now you need it to run *at least* once

```
for (i=0, i <10, i++>) {
  doSomething();
}
```

The condition is made up of three statements: 

1.  Initalization: create a variable (i) and set it equal to 0
```
i = 0
```
2. Condition: the loop will continue to run until it reaches a specified number (in this case, 10).
```
i < 10
```
3. Update: every time the loop runs the statement in the curly braces, it adds one to the counter
```
i++
````
When the condition is no longer true, the loop ends. 