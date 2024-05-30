# API End Points

- Functions to get set data from backend interfaces
- (?) It could also be described as series of REST API end points, but if described as functions it has the advantage that it abstracts from the client server communication implementation. Eg you could use socket, graphQL etc..) (?)

**Artefact**

- functions names and parameters (interface)

eg

```jsx
getPost(apiKey,userId, postId)
```

> What is the data flow (API) / User flow — List of all API’s i.e what kind of APIs we need and general user flow, where will the user click, and what will happen.

from [https://bootcamp.uxdesign.cc/front-end-system-design-guide-9a11381f5e81](https://bootcamp.uxdesign.cc/front-end-system-design-guide-9a11381f5e81)

What does the component’s API look like?

What does the backend API look like?

from [https://performancejs.com/post/hde6d32/The-Best-Frontend-JavaScript-Interview-Questions-](https://performancejs.com/post/hde6d32/The-Best-Frontend-JavaScript-Interview-Questions-)

Here you can define the functions used on the client eg 

```jsx
getPost(apiKey,userId, postId)
```

and/or REST end points (?)

```jsx
/user/:userId/posts/:postI
```