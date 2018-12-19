---
title: 'The Mousemove Event'
author: Eduardo
layout: post
categories:
  - Blog post
tags: javascript javascript30
---
There are many other blog posts out there that explain the mousemove event better than I could even attempt to. But in this post, I want to talk about, what I found to be, a quirky behavior from the mouseover event.

I came accross this behavior while completing day 16 of [JavaScript 30](https://javascript30.com/): the mouseover event's `offsetX` and `offsetY` properties consider the element you're hovering over **even** if you're listening on another specific element. "What?" Yeah, I know. Let me explain.

Let's say you have a `<div>` and this is the element on which you're adding an event listener for 'mousemove'. And let's also say that you're console logging the `offsetX` and `offsetY` properties. If this `<div>` has any children elements, the `offsetX` and `offsetY` properties that will be console logged will be the ones from the element being hovered; it could either be the `<div>` or one of its children, if any.

I found this to be quite peculiar.

The way around it is to **add** the `offsetLeft` and `offsetTop` values of the `<div>` to the element being hovered over. So:

```javascript
if (this !== e.target) {
    x = x + e.target.offsetLeft;
    y = y + e.target.offsetTop;
}
```

If you have any questions, ask me on [Twitter](https://twitter.com/eltorres720) or check out day 16 of [JavaScript 30](https://javascript30.com/).

Hope this helps!