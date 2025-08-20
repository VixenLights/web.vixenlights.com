---
title: Contribute to Vixen
author: Vixen Team
weight: 10
description: How to contribute to the Vixen application.
---

### Overview

Vixen is an open source project and we appreciate getting patches and contributions to make Vixen and its documentation even better.

The Vixen application code is hosted on [Github][1]. You can clone the repository to get a copy of the source code to work with.

### Development Libraries

There are a few libraries and tools that you need to have installed in order to get the application to build. Depending on how much you develop in other projects you may have these already installed.

* Windows 10 or higher.
* Visual Studio 2022 / Visual Studio Code with appropriate plugins.
* MSVC v143 VS 2022 C++ tools / C++ build tools for Visual Studio Code.
* Git >= 2.47
* Microsoft .NET 8
* Microsoft Visual C++ x64 Redistributable

Project libraries are included in the source tree, or included via Nuget. Familiarity with Nuget is necessary.

The current build target is .NET 8 Windows and Visual C++. We no longer maintain x86 builds.

See this [article][4] on Visual Studio settings you should use.

See this [article][5] for information on Git.

### Workflow

When contributing to Vixen, we track all issues and improvements in our [JIRA bug tracker][2]. Work should have an associated issue created for it. It will be necessary to have an account in JIRA so you can work with the issues. See [Lifecycle][7] of an issue for guidance on how we manage issues. When you become a contributor, we can add you to the appropriate access groups to facilite workign with the issues beyond a simple user.

You should name your branches with the JIRA issue number. i.e. VIX-2345. Any commits to the branch should start with the same issue number as well. From there follow Git guidelines for commit messages. All commit messages should strive to be useful to provide context of the change. All submissions are done through pull requests on Github. See [Branching Practices][6] for guidance on this topic.

Commit messages should be descriptive and helpful for those who do not know what you changed. Each commit message titel should start with the JIRA issue id. Beyond that, you should follow Github guildlines for formatting your commit messages. [Git Commit Message][9].

Commit message example.

VIX-1234 Fixing the invalid dialog message

* Add the correct dialog message showing the error that happened.
* Removed the info icon and replaced it with the error icon.
  
More information on how we manage JIRA can be found here. [Issue Management][3].

### Project Structure

Vixen 3 is a modular application that allows for pluggable modules to be developed for it. It is written in C# and some small parts in C++. The UI consists of a mix of Winforms and WPF. The WPF sections generally follow the MVVM pattern with most of it using CATEL for the MVVM library. Any new UI should favor WPF where appropriate. The code structure is as follows under the src folder:

* /Vixen.Common - Common components used by the application and modules
* /Vixen.Modules - Modules developed and maintained by the core team, and other contributors
* /Vixen.Application - The main Vixen application
* /Vixen.Core - The Vixen core framework 
* /Vixen.Installer - Installer projects

Conventions for development:

* The assembly name should be the name of the module (eg. TimedSequenceEditor), and
* the default namespace should be "Module.ModuleType.ModuleName". For
  example, Modules.Editor.TimedSequenceEditor.
* The build output directory should be relative to the solution directory, in a
  'Release' directory release builds and a Debug folder for Debug builds. We no longer actively support x86 builds.
  It will also depend on the type of module. For example:
  
  Vixen Modules (Release):              $(SolutionDir)\Release\Output\Module.ModuleType.ModuleName
  Vixen Common assemblies (Release):    $(SolutionDir)\Release\Output\
  Vixen Applications (Release):         $(SolutionDir)\Release\Output\
* Assembly names are handled by the Directory.Build.Props file for each module type.
  
* To reference the Vixen project (or any other projects that are needed), make sure you
  add a 'project reference', and not a "normal" reference (to the binary DLL). This will help compatibility for other developers when used in different locations. References to projects should be set so they do not copy local. This avoids assembly loader issues with multiple copies. Under Properties of the reference.
  
  * Copy Local : No
  * Include Assets: None

* NuGet packages follow the same principle as Project References. You should include the package in the Common area and allow the libraries to be deployed in that path. Then in the local project the NuGet package is added but is set not to copy the assets locally by setting the following in the properties of the library.
  * Exclude Assets : None

### Developer Group

We maintain a developer group for broader discussions on Google Groups. If you are looking to join us as a contributor, please join the Vixen Development Group and introduce yourself and decscribe your interests in contributing. We can help you get started. See the [Communty Page][8] for more information on how to connect.

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
[9]: <https://github.com/joelparkerhenderson/git-commit-message>
