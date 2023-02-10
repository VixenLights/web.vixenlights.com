---
title: Git Information
author: Vixen Team
weight: 30
description: This section covers the source code tooling.
---

### Overview

The Vixen project uses [Git][2] for our source code management. [Github][1] is our collaboration tool.

### Tools

There are many tools to work with a Git based project. You will at minimum need the Git libraries installed.

[Git SCM][2]

TortoiseGit is a UI tool that can make it easier for some to use Git. This allows you to make commits, view history, etc. without having to use the command line tools in Git itself.

[TortoiseGit][3]

[TortoiseGit Manuals][4]

Visual Studio also has support within it for Git and there are also many other plugins that provide integrations as well. You are welcome to use whatever you like and are comfortable with.

### Branching Practices

The general idea is that the master branch is, tracking the development for the next version. It's stuff that's going into the product, and will be included in the next version unless something is found to have an issue in testing.

* You should not commit code to your master branch. You should keep it up to date with the real master and make branches off of it for any new work you do. When you first decide to do work on Vixen, you should fork the master at [Github][5] to your own copy of it. You should be able to build and get a running version of Vixen from that is current. Then you can easily make branches from that to work on.

* All work should be done based off of a ticket in the [Bug Tracker][6]. When you take on work for a particular item, you should create a branch off of the current master and name it the same as the ticket you are working on. I.E. VIX-1024. This provides a clear reference back to the description of the problem or feature. In addition to this, each commit should start with the ticket number. This will allow those commits to be linked to the ticket when they are eventually merged into the master. You should ensure you have an open ticket to begin work so that this tracking can occur. Once the ticket it open and assigend to you, you can move it to start work. This will indicate to other developers you are working on the ticket. Once you complete the work, you can submit a pull request to the Vixen repository where it can be reviewed. The JIRA ticket will reflect that a pull request has been submitted. Once reviewed and approved, the ticket will transition states based on it being merged, built and closed automatically. You will not need to transition JIRA beyond the initial start work in normal circumstances. The build that corresponds to the change will be marked in the JIRA ticket along with links to the commits involved. The maintainer will close the ticket when it is merged.

* If the item you are working on will span some time and the current master gets updated with new features from other developers, you can keep your branch in sync by rebasing your changes onto the current version of the master. You would do a git pull to your master from the master branch tree first. Then you can rebase your branch onto that. This will replay your commits onto the tail of the master giving you a up to date branch. Try to avoid merging the changes in the master into your own branch as this creates a messy commit history. More information on how to rebase can be found [here][7].

* If you are collaborating with another developer, then you may want to share work on a branch. Here you can both work on the same branch shared publicly or you can merge changes between yourself. This is not very common in our development structure, so ask questions if it comes up and we can help guide you through it.

* Larger bodies of work will be conducted on a feature branch in the repository. Here something like an Epic can we worked on by multiple developers, or broken up into multiple parts and that can be assembled on the feature branch and then a singular pull request can merge the entirety of that back to master. 

[1]: https://github.com
[2]: https://git-scm.com
[3]: https://tortoisegit.org
[4]: https://tortoisegit.org/docs/
[5]: https://github.com/VixenLights/Vixen
[6]: https://bugs.vixenlights.com
[7]: https://git-scm.com/docs/git-rebase