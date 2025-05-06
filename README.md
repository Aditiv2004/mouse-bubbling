<h2>🔁 Event Bubbling in JavaScript</h2>
<p>
  Event bubbling is a fundamental concept in JavaScript related to how events propagate in the DOM hierarchy. It helps manage events efficiently.
</p>

<h3>📌 Key Points:</h3>
<ul>
  <li>🔹 When an event occurs on an element, it first triggers on that element and then propagates upward to its parent, grandparent, and so on.</li>
  <li>🔹 This process is called <strong>event bubbling</strong> because the event "bubbles up" through the DOM tree.</li>
  <li>🔹 It's the default event flow model used in most browsers.</li>
  <li>🔹 You can handle events at a higher level (like a parent div) instead of attaching listeners to every child element.</li>
  <li>🔹 To stop this upward movement of events, use <code>event.stopPropagation()</code>.</li>
</ul>

<h3>🧠 Example Scenario:</h3>
<p>
  Suppose you have a <code>&lt;button&gt;</code> inside a <code>&lt;div&gt;</code>. If you click the button:
</p>
<ol>
  <li>1️⃣ The event triggers on the <strong>button</strong>.</li>
  <li>2️⃣ Then it bubbles up to the <strong>div</strong>.</li>
  <li>3️⃣ Then continues to bubble up through <strong>body</strong>, <strong>html</strong>, and finally <strong>document</strong>.</li>
</ol>

<h3>🛑 Stopping the Bubbling:</h3>
<p>
  Use <code>event.stopPropagation()</code> in your event handler if you want to prevent the event from reaching parent elements.
</p>
