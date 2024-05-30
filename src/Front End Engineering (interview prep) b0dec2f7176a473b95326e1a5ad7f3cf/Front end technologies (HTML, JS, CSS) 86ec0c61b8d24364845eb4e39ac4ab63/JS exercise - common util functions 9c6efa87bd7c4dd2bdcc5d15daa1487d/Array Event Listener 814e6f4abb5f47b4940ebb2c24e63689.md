# Array Event Listener

```jsx
/**
 * Attaching listeners to prototyoe
 */
Array.prototype.listeners = {};
Array.prototype.addListener = function(eventName, callback) {
  if (!this.listeners[eventName]) {
    // Create a new array for new events
    // idea of an array is we can invoke all callbacks
    this.listeners[eventName] = [];
  }
  this.listeners[eventName].push(callback);
};
// New push Method
// Calls trigger event
Array.prototype.pushWithEvent = function() {
  const size = this.length;
  const argsList = Array.prototype.slice.call(arguments);
  for (let index = 0; index < argsList.length; index++) {
    this[size + index] = argsList[index];
  }
  // trigger add event
  this.triggerEvent('add', argsList);
};
Array.prototype.triggerEvent = function(eventName, elements) {
  if (this.listeners[eventName] && this.listeners[eventName].length) {
    this.listeners[eventName].forEach(callback =>
      callback(eventName, elements, this)
    );
  }
};
// example
const a = [];
a.addListener('add', (items, args) => {
  console.log('items were added', args);
});
a.addListener('add', (items, args) => {
  console.log('items were added again', args);
});
a.pushWithEvent(1, 2, 3, 'a', 'b');
console.log(a);
a.pushWithEvent('hello');
a.pushWithEvent(55);
setTimeout(() => {
  a.pushWithEvent('delayed');
}, 5000);

```

[JS Vault | A Collection of tricky JS interview questions](https://jsvault.com/array-listener)