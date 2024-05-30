# (Web & Service) Workers

[WebWorkers]((Web%20&%20Service)%20Workers%20939885eef3eb4dfcae53d370d678e965/WebWorkers%20571387a97d8d41b9b37558708117a400.md)

[Service workers]((Web%20&%20Service)%20Workers%20939885eef3eb4dfcae53d370d678e965/Service%20workers%20bbea895547ac4985aef8b2d45c93b7cd.md)

[Workers overview](https://web.dev/workers-overview/)

## Difference between service workers and web workers

> There is a big difference in what they are intended for:

**Web Workers**
Web Workers provide a simple means for web content to run scripts in background threads. The worker thread can perform tasks without interfering with the user interface. In addition, they can perform I/O using XMLHttpRequest (although the responseXML and channel attributes are always null). Once created, a worker can send messages to the JavaScript code that created it by posting messages to an event handler specified by that code (and vice versa.)
[Source - Using Web Workers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers)

**Service Worker**
Service workers essentially act as proxy servers that sit between web applications, and the browser and network (when available). They are intended to (amongst other things) enable the creation of effective offline experiences, intercepting network requests and taking appropriate action based on whether the network is available and updated assets reside on the server. They will also allow access to push notifications and background sync APIs.
[Source - Service Worker API](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API)

So Web Workers are handy to run expensive scripts without causing the user interface to freeze, while Service Workers are useful to modify the response from network requests (for example, when building an offline app).

[What can service workers do that web workers cannot?](https://stackoverflow.com/questions/38632723/what-can-service-workers-do-that-web-workers-cannot)

Service worker, based on web worker. 

related to caching, 

act as a proxy between your page and the requested server

setup online behaviour 

eg used in firebase cloud messaging on web, to delivery message to client. sitting in background constantly listening then updating the UI.

[What's the difference between a Web Worker and a Service Worker? #AskFirebase](https://youtu.be/Yq32eUYg6Lc?t=123)