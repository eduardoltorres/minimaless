---
title: 'Portfolio Update'
author: Eduardo
layout: post
categories:
  - Blog post
tags: personal-projects jquery lof 
---
I have a dilemma in regard to how I write blog posts in The Leap Of Faith: I want to deliver high quality content for others to benefit from and at the same time journal my experience.

There is a significant difference for the user. It's not the same if they see "Today I Worked With..." as a post title versus "How To Work With React Hooks". While I can definitely talk about both in the same post, talking about a specific topic limits my ground to share everything I did during my day. What should I do? 🤔

#### Updates To My [Portfolio](http://www.eduardoltorres.com)

Today I spent at least 4 hours trying to set up a jQuery [toast plugin](https://github.com/kamranahmedse/jquery-toast-plugin). Like most 4 hours "bugs" the issue was nonesense: corrupted CDN links.

After some user feedback, I decided to change the behavior of the *Explore* button from my [portfolio](http://www.eduardoltorres.com). It seems that many people didn't realize that its purpose was to *fade in* the navbar's opacity from 0 to 1. That's what I used the plugin for. Go [check it out](http://www.eduardoltorres.com)!

I also modified the possible responses for the contact form: a success and an error page. 

Before, it wasn't really that friendly: after the message was submitted, the page was reloaded and the user had to scroll all the way down to see a "Email has been sent" message on the contact form. Yuck! Now the person gets a nice and personally designed message. 🙃

If for some reason there's an error, the user will also get a custom response and not an ugly [Heroku](https://heroku.com) error. Go be friendly and [send me a message](http://www.eduardoltorres.com) so you can see! 😄

Lastly, I added a temporary favicon while I design a logo. No rush on this one though.

Progressively I will continue to update my portfolio to add other features such as https and [the intersection observer I was struggling with before]({{site.url}}/the-intersection-observer/).

jQuery tip: when adding script tags to your HTML file, the chronological order should be as follows at the end of your `<body>`:
- jQuery
- jQuery plugin
- your main js file (e.g. index.js, app.js)