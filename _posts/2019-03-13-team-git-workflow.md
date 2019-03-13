---
title: "Team Git Workflow"
author: Eduardo
layout: post
categories:
  - Blog post
tags: chingu git
---

Today I spent about 3 hours trying to figure out a coherent git workflow for a team (spoiler: I don't have it yet). I believe this "team git workflow" is properly called [continuous integration](https://en.wikipedia.org/wiki/Continuous_integration).

I discussed the following approach with other web developers:

_So let's say I just cloned my team's repo that has a `master` and `dev` branch. I'm in my terminal and locally I have a `master` and `dev` branch. I'm currently on `dev`. Does this git workflow make sense?_

- _Locally, I create a new `feature` branch to implement a feature: `git checkout -b feature`_
- _I implement the feature and commit: `git add .` `git commit -m "implement feature"`_
- _I change to my local dev branch: `git checkout dev`_
- _I pull changes from the remote `dev` branch in case a teammate pushed any changes: `git pull origin dev` (if there's a merge conflict locally, I solve it)_
- _I merge my `feature` branch into my `dev` branch: `git merge feature`_
- _I push my `dev` branch to the remote repo's `dev` branch: `git push origin dev`_
- _Rinse and repeat_

The response I got was of general approval with a couple of constructive remarks. The first and most pertinent one is that a Pull Request (PR) review should be implemented in the workflow. The other and less pertinent one is that the local merging of the `develop` and `feature` branches is unnecessary.

Anyway, I will share a few resources that helped me figure out the above workflow but, like I said, there's a lot of room for improvement so take it with a grain of salt. I will update whenever I feel more confident with this dynamic.

Resources:

- [This](https://chingu.gitbook.io/cohort/cohort-resources/hard-skills/git-+-github-resources) is the git workflow section from the [Chingu](https://chingu.io) Handbook with a few resources
- The other one is [this](https://nvie.com/posts/a-successful-git-branching-model/) which I apply in my personal projects
