---
title: "How to Create an Array of Specific Length?"
author: Eduardo
layout: post
categories:
  - Blog post
tags: javascript studies
---
If you want to create an array of a certain length you'll need to use the `Array.from` method. This is how it would look if you wanted to create an array with length of 50:

```javascript
Array.from({ length: 50 });
```

The method's optional second parameter is a `map` function. Check more about `Array.from` [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from).

#### What I've Been Doing
[The other day]({{site.url}}/my-airplane-workflow/), I mentioned that I almost completely binged Wes Bos' CSS grid course. Well, every morning I have been taking 30 minutes to watch a video or two. I should be done with it in the next couple of days.

Every morning, I'm also taking 30 minutes to solve a [HackerRank](https://www.hackerrank.com/) exercise.

Yesterday, I finished my [rock, paper, scissors](https://eduardoltorres.github.io/rock-paper-scissors/) game project. This one definitely gave me a confidence boost and I really gave my all to make that code as clean as possible.

Next projects lined up are a pomodoro timer, a to-do list (perhaps I get into `localStorage` here), and a Tic Tac Toe. I've set a deadline to be done with these 3 projects by the end of the month.

I am still debating whether I should get into some Sass, jQuery and Boostrap in the mornings, after I'm done with the grid course, and integrate these with the projects. This one sounds good to me...