# Manipulating done elements

Traversing the DOM in vanilla JS 

- [ ]  Selecting or finding nodes using `document.querySelector` and in older browsers `document.getElementsByClassName`.
- [ ]  Traversal up and down – `Node.parentNode`, `Node.firstChild`, `Node.lastChild` and `Node.childNodes`.
- [ ]  Traversal left and right – `Node.previousSibling` and `Node.nextSibling`.
- [ ]  Manipulation – add, remove, copy, and create nodes in the DOM tree. You should know operations such as how to change the text content of a node (`Node.innerText`)and toggle, remove or add a CSS classname (`Node.classList.toggle`).
- [ ]  Performance – touching the DOM can be expensive when you have many nodes, you should at least know about document fragments and node caching.

[Manipulating documents - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Manipulating_documents)

[DOM Manipulation - Lydia Hallie](https://www.theavocoder.com/complete-javascript/2018/12/20/dom-manipulation)

## Selecting nodes

```jsx
document.querySelector()
```

[Locating DOM elements using selectors - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_object_model/Locating_DOM_elements_using_selectors)

## Traversal

```jsx
// Traversal up and down
Node.parentNode()
Node.firstChild()
Node.lastChild() 
Node.childNodes()

// Traversal left and right
Node.previousSibling()
Node.nextSibling()
```

[](https://www.qualitestgroup.com/resources/knowledge-center/how-to-guide/traverse-dom/)

Example of traversal in action 

## Manipulation

### Change the text content of a node

```jsx
Node.innerText = text;
```

[HTMLElement.innerText - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/innerText)

[HTML DOM innerText Property](https://www.w3schools.com/jsref/prop_node_innertext.asp)

### Add css class name

```jsx
Node.classList.add("mystyle");
```

[How To Add a Class Name](https://www.w3schools.com/howto/howto_js_add_class.asp)

### remove css class name

```jsx
Node.classList.remove("mystyle");
```

[How To Remove a Class Name](https://www.w3schools.com/howto/howto_js_remove_class.asp)

### Toggle css class name

```jsx
Node.classList.toggle("mystyle");
```

[How To Toggle Between Class Names](https://www.w3schools.com/howto/howto_js_toggle_class.asp)