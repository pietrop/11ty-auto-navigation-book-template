# Merge two json objects

Clarifying questions:

- Preferences on how to handle key collision in the merge?

# 1 - JS for loop

```jsx
const result = {};
let key;

for (key in obj1) {
  if(obj1.hasOwnProperty(key)){
    result[key] = obj1[key];
  }
}

for (key in obj2) {
  if(obj2.hasOwnProperty(key)){
    result[key] = obj2[key];
  }
}
```

# **2 - `[Object.keys()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)`**:

```jsx
const result = {};

Object.keys(obj1)
  .forEach(key => result[key] = obj1[key]);

Object.keys(obj2)
  .forEach(key => result[key] = obj2[key]);
```

# **3 - `[Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)`**

```jsx
const result = Object.assign({}, obj1, obj2);
```

# **4 - Spread Operator `[...](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)`**

Note that this option overrides common values. Eg does not handle key collisions.

```jsx
const result = {
  ...obj1,
  ...obj2,
};
```

from

[How to join two JavaScript Objects, without using JQUERY](https://stackoverflow.com/questions/21450060/how-to-join-two-javascript-objects-without-using-jquery)