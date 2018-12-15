---
title: 'The Intersection Observer API [bug is dead!]'
author: Eduardo
layout: post
permalink: /the-intersection-observer-api-bug-is-dead/
categories:
  - Blog post
tags: javascript bugs js30
---
#### On JS30:
Just a quick note to share that easter eggs exist on websites. Today’s (day 12) JS30 project was on creating an easter egg that can be accessed only with a secret code. I think [BuzzFeed](https://www.buzzfeed.com/) has one, if you want to check it out.

#### The Intersection Observer:
If you don’t know what this is, [check it out](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API). Firing functions when the window intersects with a DOM element seems pretty useful, if you ask me. Warning: not all browsers support this technology.

In the end, **I** was the bug. The malfunctioning didn’t have anything to do with the API’s code, but with my HTML. For some useless reason, I was wrapping my navbar's `<li>` with `<a>` tags. I don’t know why, but this avoided the API’s `threshold` property to function adequately.

If you’ve been with a bug for days, patience my little grasshopper.

_Maybe the bug is not where you think it is._
  
-Ed