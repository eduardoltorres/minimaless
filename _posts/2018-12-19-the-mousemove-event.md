---
title: 'The Mousemove Event'
author: Eduardo
layout: post
categories:
  - Blog post
tags: javascript js30
---
There are many other blog posts out there that explain the mousemove event better than I could even attempt to. But in this post, I want to talk about, what I found to be, a quirky behavior from the mouseover event.

I came accross this behavior while completing day 16 of [JavaScript 30](https://javascript30.com/): the mouseover event's `offsetX` and `offsetY` properties consider the element you're hovering over **even** if you're listening on another specific element. "What?" Yeah, I know. Let me explain.

Let's say you have a `<div>`. This is the element on which you're adding an event listener for 'mousemove'. And let's also say that you're console logging the `offsetX` and `offsetY` properties every time you mousemove. If this `<div>` has any child elements, the `offsetX` and `offsetY` properties that will be console logged will be the ones from the element being hovered overed and not necessarily the `<div>`'s. It could either be the `<div>`'s or one of its children's, if any.

I found this to be quite peculiar.

The way around it is to **add** the `offsetLeft` and `offsetTop` values of the `<div>` to the element being hovered over. So:

```javascript
if (this !== e.target) { 
/* Remember that 'this', when listening on an event,
will always be the element on which we're listening to the event.
In this case, the div. */
    x = x + e.target.offsetLeft;
    y = y + e.target.offsetTop;
}
```

If you have any questions, ask me on [Twitter](https://twitter.com/_eduardoltorres) or check out day 16 of [JavaScript 30](https://javascript30.com/) for the full exercise.

Hope this helps!