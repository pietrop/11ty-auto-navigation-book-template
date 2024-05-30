# Event delegation

Event delegation is setting a listener on the parent element to listen for events on the child elements. Via `event.target`

> Capturing and bubbling allow us to implement one of most powerful event handling patterns called event delegation.

The idea is that if we have a lot of elements handled in a similar way, then instead of assigning a handler to each of them – we put a single handler on their common ancestor.

In the handler we get `event.target` to see where the event actually happened and handle it.

from 

[Event delegation](https://javascript.info/event-delegation)

[Event Delegation](https://davidwalsh.name/event-delegate)

[Event Delegation in Javascript | UI/Frontend Interview Question](https://youtu.be/3KJI1WZGDrg)