---
title: 'The Intersection Observer'
author: Eduardo
layout: post
permalink: /the-intersection-observer/
categories:
  - Blog post
tags: javascript bugs personal-projects
---
Today I have gotten to know a bit more intimately the [intersection observer](https://developer.mozilla.org/en-US/docs/Web/API/IntersectionObserverEntry). This is not a tutorial on how to use it, but more into understanding its behavior or at least part of it. I'll express it through a real example.

Highlighting navbar items when clicked it's not tricky. Scrolling to that section either. However, if you're scrolling and you want to highlight the navbar item that points to the visible section, things get a bit trickier.

Apparently, old school web developers used to listen for the 'scroll' event, calculate the window's distance from the top and compare it with the section's distance from the top plus its height...or something like that. Supposedly this was problematic because scrolling events are fired too often and this could turn out to be counterproductive. Enter the intersection observer.

One of the (problematic [for me]) characteristics of the intersection observer is that it considers the intersection of a section when its beginning starts to be visible and its ending invisible. That's not a problem if you're scrolling down or up one way. Each section's respective navbar item will turn on and off when visible or invisible. The problem comes when you change direction in the middle of a section.

Since the intersection observer has not detected that the section is “out” or invisible, then it won’t produce any effect. I posted a [question](https://stackoverflow.com/questions/53746874/intersection-observer-highlight-current-section) on Stack Overflow regarding this problem. I've also asked in a few other places such as Twitter and a Discord channel. If you’ve never posted a question, it feels pretty cool. Formatting it and making it look decent gives you a sense of accomplishment or at least that was my experience. Anyway, I’ll keep you posted on how I solved this issue. Possibly even make a video tutorial on it.