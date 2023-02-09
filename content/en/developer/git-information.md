---
title: Git Information
author: Vixen Team
weight: 10
---

### Tools

The Vixen project uses Git for our source code management. Github is our collaboration tool.

There are many tools to work with a Git based project. Yo uwill at minimum need the Git libraries installed.

[Git SCM][2]

TortoiseGit is a UI tool that can make it easier for some to use Git. This allows you to make commits, view history, etc. without having to use the command line tools in Git itself.

[TortoiseGit][3]

[TortoiseGit Manuals][4]

Visual studio also has support within it for Git and there are also many other plugins that provide integrations as well. You are welcome to use whatever you like and are comfortable with.

### Branching Practices

The general idea is that the master branch is, tracking the development for the next version. It's stuff that's going into the product, and will be included in the next version unless something is found to have an issue in testing.

(a) You should not commit stuff to your master branch. You should keep it up to date with the real master and make branches off of it for any new work your do. When you first decide to do work on Vixen, you would fork the master at [Vixen Source][5] to your own copy of it. You should be able to build and get a running version of Vixen from that is current. Then you can easily make branches from that to work on. Tools like TortoiseGit make it easier to manage changing branches and committing work.

As a maintainer, even I do not commit any work directly to the master branch. All commits on the master branch are actually merges of work from other branches.

(b) All work should be done based off of a ticket in the [JIRA Bug Tracker][6]. When you take on work for a particular item, you should create a branch off of the current master and name it the same as the ticket you are working on. I.E. VIX-1024. This provides a clear reference back to the description of the problem or feature. In addition to this, each commit should start with the ticket number as well. This will allow those commits to be linked to the ticket when they are eventually merged into the master. You should ensure you have an open ticket to begin work so that this tracking can occur. Once the ticket it open and assigend to you, you can move it to start work. This will indicate to other developers you are working on the ticket. Once you complete the work, you can submit a pull request to the Vixen repository where it can be reviewed. The JIRA ticket will reflect that a PR has been submitted. Once reviewed and approved, the ticket will transition states based on it being merged, built and closed automatically. You will not need to transition JIRA beyond the initial start work in normal circumstances. JIRA will track the changes when they are committed to the main repository. The build that corresponds to the change will be marked in the JIRA ticket along with links to the commits involved.

(c) If the item you are working on will span some time and the current master gets updated with new features from other developers, you can keep your branch in sync by rebasing your changes onto the current version of the master. You would sync your copy of the master from the master branch tree first. Then you can rebase your branch onto that. This will replay your commits onto the tail of the master giving you a up to date branch. Try to avoid merging the changes in the master into your own branch as this creates a messy commit history. More information on how to rebase can be found [here][7].

(d) If you are collaborating with another developer, then you may want to share work on a branch. Here you can both work on the same branch shared publicly or you can merge changes between yourself. This is not very common in our development structure so ask questions if it comes up and we can help guide you through it.

(e) If you want to have a play with someone else's branch (to test, or add features to it), as long as they have pushed a copy of it out to their public repository, then you can always make your own branch at that point, and go from there. For example, Jeff might take a look at Jon's _VersionControl_ branch, and make a new one for himself, called _copy-branch_ or something. He can do some more work to do with the version control, maybe updating stuff, adding a new feature, etc. Then, if Jon likes it, he can merge from Jeff's VC branch back into his own VC branch. (since it's all separate to 'master', he can do what he likes with it.) Once all the work is done between the two developers, the version with all the changes compiled together can be merged into the master.

(f) When work is complete on a branch, That branch should be pushed to your public repository and a pull request against the Vixen master created to indicate it is ready to be reviewed and merged.

[2]: https://git-scm.com
[3]: https://tortoisegit.org
[4]: https://tortoisegit.org/docs/
[5]: https://github.com/VixenLights/Vixen
[6]: https://bugs.vixenlights.com
[7]: https://git-scm.com/docs/git-rebase