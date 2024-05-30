# Long-Polling vs WebSockets vs Server-Sent Events

[Long-Polling vs WebSockets vs Server-Sent Events - Grokking the System Design Interview](https://www.educative.io/courses/grokking-the-system-design-interview/gx7wZzWn5Vj)

## Long-Polling

The client sends request to the server to check if anything has change

but the server, if nothing has changed, holds on to the request until there's something new and then it responds.

This might time out, and then the client sends another request(?)

[Long polling](https://javascript.info/long-polling)

[What is HTTP Long Polling?](https://www.pubnub.com/blog/http-long-polling/)

## WebSockets

[WebSocket](https://javascript.info/websocket)

## Server-Sent Events

[Server Sent Events](https://javascript.info/server-sent-events)