1.What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Ans - GetElementById - This method selects a single element based on its unique id. Because IDs must be unique in a Docs and it always return one element. 

getElementsByClassName - This selects all elements that have a specific class name. It is a HTNL collection and it is an array-like object.

querySelector / querySelectorAll - These are the most flexible methods.  Queryselector returns the one and first matching element . On the other hand, querySelectorAll  returns all matching elements in a nodelist.

2.How do you create and insert a new element into the DOM?
Ans - i Use "document.createElement('tagName')" to create an element.Then insert a new element by suing "append.chhild".

3.What is Event Bubbling? And how does it work?
Ans-Event bubbling is a JavaScript mechanism where an event triggered on a child element triggers handlers on its parent and ancestor elements, propagating upward through the DOM tree to the root. It acts like a bubble rising in water, starting from the target element. When an event happens on an element, it first runs the handlers on it, then on its parent, then all the way up to other ancestors.

4.What is Event Delegation in JavaScript? Why is it useful?
Ans- Event Delegation is a clever technique in JavaScript that leverages Event Bubbling. Instead of adding an event listener to every single child element,add one single listener to their parent. It is useful for If i have a list of 1,000 items, adding 1,000 listeners then slow down the browser. With delegation,i only use one listener for better perfomance .And don't have to write loops to attach listeners to every element.

5.What is the difference between preventDefault() and stopPropagation() methods?
Ans - While both methods are used to "stop" something from happening in an event, they handle two completely different behaviors: Action vs Flow.
preventDefault() : it stopping the form from refreshing page .It also stopping a link <a> from opening a URL. This method stops the browser's default behavior associated with an event. It does not stop the event from bubbling up the DOM.

stopPropagation() : It commonly uses for Clicking a "Delete" button inside a card without triggering the card's click event. This method stops the event from bubbling up to parent elements. It prevents the event from "traveling" further up the DOM tree.

