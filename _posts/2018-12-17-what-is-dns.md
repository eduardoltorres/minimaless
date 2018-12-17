---
title: 'What Is DNS?'
author: Eduardo
layout: post
categories:
  - Blog post
tags: hosting lof personal-projects
---
Go check out [this](https://howdns.works/) amazing explanation of what it is. I'm serious. Even if you don't care what DNS is, you should check that out. Once you start reading, you'll end up wanting to know.

[Yesterday]({{site.url}}/domains-hosting-dns-and-name-servers/), I narrated the beginning of my bloddy battle against the hosting monster. And it's not over yet!⚔️ Still, I want to share some resources I've been checking out in case you have more luck than me in understanding how they work.

The following is what I think I understand: [Zone Vision](https://zone.vision/#/) I got from the [Heroku](https://heroku.com/) documentation. What it does, basically, is that it inspects the **real** DNS zones of your domain even before the changes are reflected. This should be pretty straightforward. If you don't understand what I'm talking about, you have homework: check out my previous [post]({{site.url}}/domains-hosting-dns-and-name-servers/), in which I talk about the time it takes for DNS changes to be reflected, and check out the link I provided above for the explanation on [how DNS works](https://howdns.works/).

[What's My DNS](https://www.whatsmydns.net/) does more or less the same thing. Play with the both of them and see which one you like most.

Lastly, if all else fails after 48 hours, contact your domain name registrar or wait a few days till I figure it out and am able to explain it to you.

In case you're checking constantly and are experiencing some weird behavior from your domains after changing your DNS, this is what has happened to me (maybe it can shed some light on your issue): after more than 24 hours, one of my domains seems to be working intermittently. Only if I visit from my computer though. If I visit from my phone, it doesn't work. This is my [portfolio](http://eduardoltorres.com) page which I'm trying to point to Heroku. If you try to visit the day I posted this blog post, you'll see that it is still not available.

The Leap Of Faith, the one you're reading from right now, started working after a couple of hours. This one, however, has the quirky behavior that it only works if you type http://theleapofaith.com and not if you type www.theleapofaith.com. I don't know about you, but after 48 hours I'm definitely contacting [my domain name registrar](https://www.namesilo.com/).