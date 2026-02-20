---
title: Sandbox Testing
author: Vixen Team
weight: 50
---

## Overview

Sometimes it is neccessary to do testing in an isolated environment. We have provided some configuration to enable testing Vixen in an isolated windows environemnt.

## Sandbox Tools

If you are running one of the pro versions of Windows, you can utilize the Windows Sandbox to test your builds in an isolated environment. This can be very useful to simulate what a first time user might experience. This is very useful for testing the installer or new versions that may have breakign changes that you want to avoid corrupting your real profiles. See the [Sandbox Testing][github-sandbox] in the Vixen source project for further information on how to do this.

[Windows Sandbox][windows-sandbox]

[Windows Sandbox Configuration][windows-sandbox-config]

[github-sandbox]: https://github.com/VixenLights/Vixen/tree/master/sandbox
[windows-sandbox]: https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/
[windows-sandbox-config]: https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/windows-sandbox-configure-using-wsb-file