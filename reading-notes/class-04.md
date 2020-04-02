# HTML Layout

HTML treats each element as if it were in it's own box.  Each element is either a **block** element or an **inline** element.  

**Block level element**
- Starts on a new line

**Inline level element**
- Flows inbetween surrounding text

If one block level element sits inside another block level element, the outer box is known as the **parent** element

# CSS Positioning

**Normal Flow**
- Every block level element appears on a new line

**Relative Positioning**
- Shifts the element from the top, right, bottom, or left, in relation to where it would have normally been placed

**Absolute Positioning**
- Positions the element in relation to its containing element 

**Fixed Positioning**
- Form of absolute positioning
- Positions element in relation to browser window, as opposed to the containing element

**Floating Element**
- Takes element out of normal flow as positions to the far left or right of containing block

# JavaScript Functions

Functions let you group a series of statements together to perform a specific task.  To create, or **declare** the function:

```
function sayHello() {
  document.write('Hello');
}
```
You then must **call the function**:
```
sayHello();
```
If the function needs specific information to perform the task, you give it **parameters**:
```
function getArea (width, height) {
  return width * height;
}
```
## Scope

The location where you declare your variable can affect where it can be used. 

**Local Scope**: If you create a variable inside a function, it has *local* scope and can only be used inside that function

**Global Scope**: If you create a variable outside of a function, it has *global* scope and can be used anywhere in the file

*Note: global variables use more memory*


# Pair Programming

Pair programming involves two people: the **driver** and the **navigator**.   The driver types while the navigator users their words to guide the driver.

Pair programming touches on the four fundamental skills of learning a language:

1. Listening: listening and interpreting the vocabulary
2. Speaking: using the correct words to communicate an idea
3. Reading: understanding what written language intends to convey
4. Writing: producing from scratch 

## Top six reasons to pair program

1. Greater efficiency 
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness
