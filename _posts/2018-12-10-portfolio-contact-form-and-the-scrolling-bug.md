---
title: 'Portfolio Contact Form And The Scrolling Bug'
author: Eduardo
layout: post
permalink: /portfolio-contact-form-and-the-scrolling-bug/
categories:
  - Blog post
tags: javascript bugs blog lof
---
#### On Portfolio:
Node.js is really a bunch of middleware. At least that was my experience today while setting up the back end for my portfolio’s contact form. I set it up following an awesome and easy to follow [tutorial](https://www.youtube.com/watch?v=nF9g1825mwk) from Traversy. Even though I didn’t finish polishing the design, I managed to get it working. Tomorrow I should be done with the form’s design and ready to work out the responsiveness of the website.

Last but not least—and before deployment—I still have one bug that won’t die. I call it the scrolling bug. Whenever you scroll on the page, the sticky navbar’s items light up depending on which section of the page you’re on. It’s a one page website. The way I set it up was by using some math to calculate the `pageYOffset` of the window and compare it with the `offsetTop` of the section. If the window is between the section’s `offsetTop` and the section's `offsetTop + offsetHeight` then apply the `current` class.

Sounds good and logical and it works, but it toggles the class a tiny bit too late. I want to get that transition to run as smooth as possible. However, I do think I know where the bug is and I believe it to be in the CSS. Instead of setting a height, I’ve been tweaking with the apparent height of each section by applying margin and padding to the section’s headers. This extra margin and padding, I suspect, is not considered part of the section's height. Now you guess the rest. Tomorrow that bug is dead for sure.

#### On The Leap Of Faith:
I’ve gotten the idea for how the next Leap of Faith could be once I get a job as a web developer or an equivalently credible status. I will create a roadmap for new aspiring self-taught web developers. In case you’re reading this from the future and are an aspiring self-taught web developer, this idea came to mind by asking myself “what do I need now as an aspiring self-taught web developer?” I thought that a roadmap would be useful, but more specifically, a timeline and a schedule based on those of someone who became a web developer.

The idea is to keep these posts that have already been published, just as they are, and produce curated graphs and illustrations on what I did and I didn’t, on what I said I would do and what I said I wouldn’t, but specially on what I did each day. The posts would be here as reference. Whenever someone is examining one of the graphs or schedules and wants to refer to a post to see what exactly I did on that day, they will be able to. Starting from now on, I’ll start writing with that end in mind. This, aspiring web developer, is for you.