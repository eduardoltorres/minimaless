---
title: 'Sticky Nav'
author: Eduardo
layout: post
categories:
  - Blog post
tags: javascript js30
---
Have you ever wondered how to make a navbar sticky when it does **not** start at the top of the webpage? Or perhaps you've asked yourself how to animate this transition from `position: static` to `position: fixed`?

If this is not clear yet, [check it out](https://eduardoltorres.github.io/sticky-nav/) and then come back (if you're curious about the code, you can check it [here](https://github.com/eduardoltorres/sticky-nav)).

[Wes Bos](https://wesbos.com/) explains it better than I would so if you want to code along I recommend day 24 of [JavaScript 30](https://javascript30.com). In this post, I want to share the most important takeaways for me from this lesson:

- `position: fixed` "leaves a hole"
- add class to parent element, not to specific element

The "trick" behind this transition is to change the navbar's `position` from default or `static` to `fixed`. When you do this, the element ceases to take the space it once did and the rest of the page's elements "move up". In other words, the rest of page behaves as if there was not an element there taking up space. The way to remedy this is by adding some `padding-top` to the `body` or whichever parent element requires it.

You might think that it is the navbar directly that one would modify. This is another trick: modify the parent element. In this case, add the `.fixed-nav` class to the `body` and not the navbar. Why? Because that way you can then modify other child elements based on the parent's (the `body` in this case) status or class. In this case, we modified the navbar's and logo's behavior by styling them whenever the `body` had a class of `.fixed-nav`.

```css
.fixed-nav nav {
  position: fixed;
  box-shadow: 0 5px rgba(0, 0, 0, 0.1);
}
.fixed-nav li.logo {
  max-width: 500px;
}
```

These are clean, efficient and creative ways to handle popular problems.

What do you think? Let me know on [Twitter](https://twitter.com/eltorres720).