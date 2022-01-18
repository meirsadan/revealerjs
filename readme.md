# Revealer.js

## What does it do?

Revealer.js detects special attributes that trigger simple interactions – hide/show or toggle a certain class name.

It is intended for use by HTML/CSS developers who have not yet mastered JavaScript.

## How to use it?

1. Download `revealer.js` and put it in your website's directory.

2. Link to `revealer.js` by adding this code before the closing `</body>` tag:

```js
    ..
    <script src="revealer.js"></script>
</body>
</html>
```

3. Add `data-click` or `data-hover` attributes to elements you want to use as triggers. They should contain a selector string that points to the element you want to be triggered (for example: `#my_id` or `.myclass`).

```js
    <button data-click="#hiding_element">Hide or show me!</button>
    <div id="hiding_element">I will hide/show!</div>
```

4. Add the optional `data-click-class` and `data-hover-class` to toggle a certain class name instead.

```js
    <button data-click="#element" data-click-class="red">Click to make the element red!</button>
    <div id="element">I will become red!</div>
```
