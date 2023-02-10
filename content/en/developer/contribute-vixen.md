---
title: Contribute to Vixen
author: Vixen Team
weight: 10
description: How to contribute to the Vixen application.
---

### Overview

Vixen is an open source project and we love getting patches and contributions to make Vixen and its docs even better.

The Vixen application code is hosted on [Github][1]. You can clone the repository to get a copy of the source code to work with.

### Development Libraries

There are a few libraries and tools that you need to have installed in order to get the application to build. Depending on how much you develop in other projects you may have these already installed.

* Windows 10 or higher.
* Visual Studio 2022
* Git
* Microsoft .NET Framework 4.8
* Microsoft Visual C++ 2019 x86 Redistributable
* Microsoft Visual C++ 2019 x64 Redistributable

The current build target is .NET 4.8 and Visual C++ 2019, but we are actively migrating to .NET 6 and will be using Visual C++ 2022.

See this [article][4] on Visual Studio settings you should use.

See this [article][5] for information on Git.

### Workflow

When contributing to Vixen, we like to track all issues and improvements in our [JIRA bug tracker][2]. Work should have an associated issue created for it. It is a good idea to have an account in JIRA so you can work with the issues. See [Lifecycle][7] of an issue for guidance on how we manage issues.

You should strive to name your branches with the ticket number. i.e. VIX-2345. Any commits to the branch should start with the ticket number as well and then follow Git guidlines for commit messages. All submissions are done through pull requests on Github. See [Branching Practices][6] for guidance on this topic.

More information on how we manage JIRA can be found [here][3].

### Creating Issues

Alternatively, if there's something you'd like to see in Vixen (or if you've found something that isn't working the way you'd expect), but you're not sure how to fix it yourself, please create an [Issue][2] in our JIRA board for anything in the application.

[1]: https://github.com/vixenlights/vixen
[2]: https://bugs.vixenlights.com
[3]: {{< ref issue-management >}}
[4]: {{< ref visual-studio >}}
[5]: {{< ref git-information >}}
[6]: {{< ref "git-information#branching-practices" >}}
[7]: {{< ref "issue-management#lifecycle-of-a-ticket" >}}
