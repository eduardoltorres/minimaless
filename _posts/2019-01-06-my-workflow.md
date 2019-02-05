---
title: 'My Workflow (Under 🚧)'
author: Eduardo
layout: post
categories:
  - Blog post
tags: productivity studies
---
[Yesterday]({{site.url}}/write-before-you-code/), I talked about some of the advantages of writing down your idea before coding. After that, I think I discovered my ideal workflow.

First I'll mention it and then I'll explain it. Here's how it goes:
- Organize idea in [Agile Trello Board](https://trello.com/b/WELsX9Hm/agile-board-example)
- Experiment feature with [Codepen](https://codepen.io) *(optional)*
- Create a git branch to implement experimented feature (I follow [this](https://nvie.com/posts/a-successful-git-branching-model/) git workflow)
- Merge, push (if desired), rinse and repeat

Okay, now a bit slower.

Organizing my idea in the Trello board is just a more sophisticated way of doing what I explained [yesterday]({{site.url}}/write-before-you-code/). [This](https://trello.com/b/WELsX9Hm/agile-board-example) Trello board has all the details.

If you're interested in planning, check it out and experiment with it. Agile is a known project management methodology for software development and many employers require you to have experience working with it.

Once you have your ideas organized and broken into bite-sized chunks, get to [Codepen](https://codepen.io) and experiment. The reason why I marked this as optional is because perhaps you're pretty sure of the ideas or really don't care much.

In my case, I like to experiment with different ideas, many of them design-wise, and changing my code or creating a branch just for that and then just reverting...it just seems like a lot of work to me. Ideally, if it's design-wise, you'll experiment with a design software, but for me Codepen does the job for now.

If you're new to git, I suggest you skip the next step and start getting comfortable with the basic commands (init, status, add, commit, push). If you're already comfortable with that, but don't know much more, then this one's for you.

Check out [this](https://nvie.com/posts/a-successful-git-branching-model/) article on the workflow (it is also linked in the Trello board). There is a [condensed version](https://flaviocopes.com/git-workflow/) from Flavio. These are enough to understand this step.

Lastly, it is for you to decide if you want to push or deploy your progress.

I just want to make one last comment of one little phenomenon that could come up and hinder your productivity: **don't worry about DRY code in the beginning**.

If you're like me, you want to implement the best practices, write clean and efficient code, etc. **Don't worry about this when you're experimenting**. You could even wait until you deploy and then clean it little by little.

You shouldn't experiment **AND** at the same time try to be efficient. Efficient code is not separate from your HTML structure, for example, and if you're manipulating the DOM, you'll be changing your structure constantly, then you'll be doing double the work: experimenting + refactoring.

What's your workflow? Let [me](https://twitter.com/_eduardoltorres) know.

P.S. why under 🚧? Well, I'm just experimenting with it🙂