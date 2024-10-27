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
* Visual Studio 2022 / Visual Studio Code with appropriate plugins.
* Git >= 2.47
* Microsoft .NET 8
* Microsoft Visual C++ x64 Redistributable
* Project libraries are included in the source tree, or included via Nuget. Familiarity with Nuget is necessary.

The current build target is .NET 8 Windows and Visual C++. We no longer maintain x86 builds.

See this [article][4] on Visual Studio settings you should use.

See this [article][5] for information on Git.

### Workflow

When contributing to Vixen, we track all issues and improvements in our [JIRA bug tracker][2]. Work should have an associated issue created for it. It will be necessary to have an account in JIRA so you can work with the issues. See [Lifecycle][7] of an issue for guidance on how we manage issues. When you become a contributor, we can add you to the appropriate access groups to facilite workign with the issues beyond a simple user.

You should name your branches with the JIRA issue number. i.e. VIX-2345. Any commits to the branch should start with the same issue number as well. From there follow Git guidelines for commit messages. All commit messages should strive to be useful to provide context of the change. All submissions are done through pull requests on Github. See [Branching Practices][6] for guidance on this topic.

More information on how we manage JIRA can be found [here][3].

### Developer Group

We maintain a develoepr group for broader discussions on Google Groups. If you are looking to join us as a comtributor, please join the Vixen Development Group and introduce yourself and decscribe your interests in contributing. We can help you get started. See the [Communty Page][8] for more information on how to connect.

### Creating Issues

Alternatively, if there's something you'd like to see in Vixen (or if you've found something that isn't working the way you'd expect), but you're not sure how to fix it yourself, please create an [Issue][2] in our JIRA board for anything in the application.

[1]: https://github.com/vixenlights/vixen
[2]: https://bugs.vixenlights.com
[3]: {{< ref issue-management >}}
[4]: {{< ref visual-studio >}}
[5]: {{< ref git-information >}}
[6]: {{< ref "git-information#branching-practices" >}}
[7]: {{< ref "issue-management#lifecycle-of-a-ticket" >}}
[8]: {{< ref community >}}
