1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Answer:

getElementById("id") → Returns one element by its id.

getElementsByClassName("class") → Returns a live collection of all elements with that class.

querySelector("selector") → Returns the first element matching a CSS selector.

querySelectorAll("selector") → Returns a static list of all elements matching a CSS selector.


2. How do you create and insert a new element into the DOM?

Ans: 1. Create the element: 
const newDiv = document.createElement("div");
2. Add content or attributes:
document.body.appendChild(newDiv);
3. Insert into the DOM:
document.body.appendChild(newDiv);

3. What is Event Bubbling and how does it work?

Ans: Event Bubbling is when an event starts from the target element and then moves upward through its parent elements until it reaches the root (document).

Example: If you click a button inside a div, the click event runs on the button first, then on the div, then on the body, and so on.

4. What is Event Delegation in JavaScript? Why is it useful?

Answer: Event Delegation is a technique where instead of adding event listeners to many child elements, you add a single event listener to a parent element and use event bubbling to catch events from its children.

* Why useful?

Saves memory (fewer listeners).

Works for dynamically added elements.

5. What is the difference between preventDefault() and stopPropagation() methods?
Ans:
preventDefault() → Stops the default browser action 
stopPropagation() → Stops the event from bubbling up to parent elements.
