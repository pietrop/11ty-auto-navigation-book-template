# Questions

[amilajack/front-end-system-design](https://github.com/amilajack/front-end-system-design)

Front end design system questions

[The Best Frontend JavaScript Interview Questions (written by a Frontend Engineer)](https://performancejs.com/post/hde6d32/The-Best-Frontend-JavaScript-Interview-Questions-)

See front end system design section at the bottom

- Q: How would you update the UI without user interaction? eg the data on the server has changed.
    - A: Pooling (long or short) or sockets
    - Sockets, the connection with the server is open. It can be heavier on the server based on threading capabilities (eg Node better then Rails)
    - Sockets get complicated with CDN is involved. Eg you have to have bypass the CDN or use a service like firebase/firestore or some push service.

- Q: How do you build a UI when the API is not fully fleshed out?
    - A: You can create an "API Contract" between API Dev and UI Dev by defining a (schema) for a json that will be returned by the API end point.