# Events

Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).

Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.

You can use event delegation to monitor for events that happen on all of the children of an element.

Whenever an element is added or removed to the DOM, it triggers a **mutation event**.  Too many mutation events can slow down the page.

Three page-level scrips to help with that:
- `DOMContentLoaded`
- `hashchange`
- `beforeunload`

# jQuery

jQuery is a JavaScript library that makes manipulating the DOM faster and easier by using simple selectors and common tasks that require less code

1) Find elements using CSS-selectors: 
`$('li.hot')`
2) Do something with the elements using jQuery methods: `$('li.hot').addClass('complete')`

When you create a selection with jQuery, it stores a reference to the corresponding nodes in the DOM tree

# Pair Programming

Six reasons to pair program:
1) Greater efficiency 
2) Engaged collaboration 
3) Learning from fellow students
4) Social skills
5) Job interview readiness
6) Work environment readiness 