---
layout: post
title: "Useful links for Learning GIT"
date: 2017-10-12
tags: resources git
---

This page is just another way for me to collect notes and some links that I have briefly visited and have found useful for learning GIT. Of course I can always run another search, but some of these links I found through recommendations or serendipity.  

I'll occasionally add to this page, but won't attempt to organize them. These exist as prompts for later review.

* [Can you explain what “git reset” does in plain english? 2010](https://stackoverflow.com/questions/2530060/can-you-explain-what-git-reset-does-in-plain-english#2530073)
* [Cannot update paths and switch to branch at the same time](https://stackoverflow.com/questions/22984262/cannot-update-paths-and-switch-to-branch-at-the-same-time)
* [How can I merge two commits into one?](https://stackoverflow.com/questions/2563632/how-can-i-merge-two-commits-into-one?answertab=active#tab-top)
* [5 good practices I follow when I code using Git](https://tech.olx.com/5-good-practices-i-follow-when-i-code-using-git-71120b57c0f5)
* [GIT Commands Tutorial](https://www.siteground.com/tutorials/git/commands/)
* [Git-it (Original, retired)](https://github.com/jlord/git-it)  
* [How to revert Git repository to a previous commit?](https://stackoverflow.com/questions/4114095/how-to-revert-git-repository-to-a-previous-commit)
* [How do I delete a Git branch both locally and remotely?](https://stackoverflow.com/questions/2003505/how-do-i-delete-a-git-branch-both-locally-and-remotely)
* [Git Branching - Basic Branching and Merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)

```
From a discussion on our CodeLouisville git channel:  

Daniel Hammond [9:22 AM]
Quick tip: `git reset --hard` is a good way to discard changes and get back to
your most recent checking. _Do not do this unless you're willing to lose files._
 (I think.)
checking -> check-in

Margeaux Spring [9:24 AM]
or if you have not yet committed `git checkout whateveryourfilename` (edited)

[9:25] or if a bunch of file changes `git checkout .` resets the files back to
previous state

Daniel Hammond [9:26 AM]
As always there's a billion different ways in git to do the same thing

Margeaux Spring
[9:29 AM] diff is `git reset --hard` functions on the complete work tree,
the `git checkout filename` is just for that file(s) updating the work tree
and leaving already staged files alone

Mark Biek [9:29 AM]
You can also do `git reset --soft` which will undo the commit but put the
changes back into your working copy.
```  

```
from Leigh Prince:

_Origin_ and _master_ refer to two different things here. *Origin* is the most
commonly-used-name for remotes and _master_ is the default name for branches.
Think of a remote as a bridge between your GitHub repo and your local repo. So…

`git push origin master`

Calls git, tells it we’re going to push, tells it which road to take, then tells
 it what payload to handle

Your remote, like your branches, can be named whatever but _origin_ is what
people usually go with  

```  
> if you make changes, and don’t either commit or stash those changes, they go with you to a branch if you check out a different branch.
