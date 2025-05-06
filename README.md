<h2>Event Bubbling in JavaScript</h2>
<p>
  Event bubbling is a concept in the DOM (Document Object Model) where an event starts from the deepest (innermost) element and then bubbles up to its ancestors (outer elements). When an event is triggered on a child element, it first runs the event handlers on that element, and then propagates the event to its parent, then grandparent, and so on up to the root element.
</p>
<p>
  This default behavior allows a single event handler to be attached to a parent element to manage events from all its children, improving efficiency. You can stop the bubbling process using the <code>event.stopPropagation()</code> method.
</p>
<p>
  <strong>Example:</strong> If you click on a button inside a div, the click event first triggers on the button and then bubbles up to the div and higher elements unless explicitly stopped.
</p>
