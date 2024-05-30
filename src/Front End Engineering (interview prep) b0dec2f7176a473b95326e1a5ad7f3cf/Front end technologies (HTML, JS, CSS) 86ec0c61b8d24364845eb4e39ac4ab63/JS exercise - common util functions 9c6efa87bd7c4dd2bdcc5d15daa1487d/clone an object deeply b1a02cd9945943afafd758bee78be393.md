# clone an object deeply

> Iterating through each object property and copying it into a new empty object

```jsx
let user = {
  name: "Alexander",
  age: 26
};

let clone = {}; // the new empty object

// let's copy all user properties into it
for (let key in user) {
  if (user.hasOwnProperty(key)) {
  clone[key] = user[key];
 }
}

// now clone is a fully independent object with the same content
clone.name = "Chinedu"; // changed the data 

console.log(user.name); // still Alexander in the original object
```

from 

[Methods for deep cloning objects in JavaScript - LogRocket Blog](https://blog.logrocket.com/methods-for-deep-cloning-objects-in-javascript/)

[What is the most efficient way to deep clone an object in JavaScript?](https://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-deep-clone-an-object-in-javascript)