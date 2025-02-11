---
title: Visual Studio
author: Vixen Team
weight: 40
---

## General Info

We use currently use Visual Studio 2019 or 2022 for development. You can use the community or free version that MS provides, or any of the higher paid versions. The current community version is quite good and is equivalent to the old Professional version. The vast majority of the code is in C#, with a small portion in C++. When you install Visual Studio, you will need the C++ build tools.

## Settings

There are a couple settings that need to be configured in Visual Studio so your code formatting will adhere to our preferred style. We use tabs instead of spaces to format our files. The following screen shot shows how you should configure the editor to do this automatically.

![Visual Studio Tab Settings](/images/docs/contribution-guidelines/visualstudio-tab-settings.png)

You should verify any changes you make are using the correct formatting. You can do this with any diff tool that shows white space in the files.

In the following diff, you can see that the new lines inserted have spaces instead of tabs for the indent formatting. This indicates that your settings are not correct and this should be fixed before continuing. If you are correcting any existing formatting issues, those should be done in separate commits specifically addressing format changes.

![Spaces vs Tabs](/images/docs/contribution-guidelines/spaces-vs-tabs.png)

## Extensions

The project uses WIX to build the installer for the application. If you are using Visual Studio, you should install the Heatwave for VS2022 extension so VS will recognize the project files. [Heatwave][2]

## Building

Within Visual Studio, you can build / run the project in debug or release mode. The release mode provides for optimized builds, where the debug builds are more geared to debugging, especially when a debugger is attached. Another option is available for additional testing. Using msbuild at the command line, you can create a full installer that can be run just like the official releases. You can read more on how to do that [here][github-installer] in the Vixen source project.

## Sandbox Tools

If you are running one of the pro versions of Windows, you can utilize the Windows Sandbox to test your builds in an isolated environment. This can be ver useful to simulate what a first time user might experience. See the [Sandbox Testing][github-sandbox] in the Vixen source project for further information on how to do this.

[Windows Sandbox][windows-sandbox]

[Windows Sandbox Configuration][windows-sandbox-config]

## Additional Tools

We also have access to some very powerful tools courtesy of some of our partners who support open source projects. One very powerful tool is [Resharper][1]. If you are an active developer and are interested in using this tool contact us on the developer list and we can discuss getting you one of our team licenses. You have to be an active developer with a verifiable commit history.

[1]: https://www.jetbrains.com/dotnet/
[2]: https://marketplace.visualstudio.com/items?itemName=FireGiant.FireGiantHeatWaveDev17
[github-installer]: https://github.com/VixenLights/Vixen/tree/master/Installer
[github-sandbox]: https://github.com/VixenLights/Vixen/tree/master/sandbox
[windows-sandbox]: https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/
[windows-sandbox-config]: https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/windows-sandbox-configure-using-wsb-file
