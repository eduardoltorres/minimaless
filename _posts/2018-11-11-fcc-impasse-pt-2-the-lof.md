---
title: 'fCC Impasse Pt. 2; the LoF'
author: Eduardo
layout: post
permalink: /fcc-impasse-pt-2-the-lof/
categories:
  - Blog post
tags: lof
---
In the end, this is the code that works and I understand it, but I still don’t understand why yesterday's code didn't work.
```javascript
for (var i = 0; i < contacts.length; i++) {
  if (name == contacts[i].firstName) {
    if (contacts[i].hasOwnProperty(prop)) {
      return contacts[i][prop];
    } return "No such property";
  }
} return "No such contact";
```
I thought (and I still think) that the problem had to do with the logical operators’ line, but this still didn’t work.
```javascript
for (var i = 0; i < contacts.length; i++) {
  if (name == contacts[i].firstName && (contacts[i].hasOwnProperty(prop))) {
    return contacts[i][prop];
  } else if (name !== contacts[i].firstName) {
    return "No such contact";
  } else if (name == contacts[i].firstName && prop !== contacts[i][prop]) {
    return "No such property";
  }
}
```
...so I added the parentheses to the second statement of the first conditional line; I tried adding them by still trying to evaluate if `prop == contacts[i][prop]` but then I realized that that is not a correct evaluation; nonetheless it didn’t work. I still don’t know why, but I don’t want to get stuck because I understand the more simpler and cleaner solution. I’ll leave it like that. I won’t spend too much time in such a simple topic. Perhaps in the future I’ll learn the lesson.

On the LoF: I updated the LoF and implemented a few new ideas (like daily posting instead of weekly or every other week). I ran into a bit of trouble pasting blocks of code in a nice and readable manner; will finish tomorrow.