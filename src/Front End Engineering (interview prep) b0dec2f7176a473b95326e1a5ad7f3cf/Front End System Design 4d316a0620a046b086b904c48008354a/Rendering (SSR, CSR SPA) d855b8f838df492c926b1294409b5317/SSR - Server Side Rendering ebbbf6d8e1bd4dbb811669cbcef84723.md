# SSR - Server Side Rendering

[What is Server-Side Rendering? (Server-side Rendering with JavaScript Frameworks)](https://youtu.be/GQzn7XRdzxY)

[Basic Features: Pages | Next.js](https://nextjs.org/docs/basic-features/pages)

[React Server Components](SSR%20-%20Server%20Side%20Rendering%20ebbbf6d8e1bd4dbb811669cbcef84723/React%20Server%20Components%20efc819a154524d2ba26d88a5dc42a643.md)

[New Suspense SSR Architecture in React 18 · Discussion #37 · reactwg/react-18](https://github.com/reactwg/react-18/discussions/37)

SSR explanation 

## React server side rendering & hydration

```jsx
import ReactDOMServer from 'react-dom/server';
ReactDOMServer.renderToString(element)
```

> If you call `ReactDOM.hydrate()` on a node that already has this server-rendered markup, React will preserve it and only attach event handlers, allowing you to have a very performant first-load experience.

[ReactDOMServer - React](https://reactjs.org/docs/react-dom-server.html)

[ReactDOM - React](https://reactjs.org/docs/react-dom.html#hydrate)

[How to Enable Server-Side Rendering for a React App | DigitalOcean](https://www.digitalocean.com/community/tutorials/react-server-side-rendering)

[How to implement server-side rendering in your React app in three simple steps](https://www.freecodecamp.org/news/server-side-rendering-your-react-app-in-three-simple-steps-7a82b95db82e/)