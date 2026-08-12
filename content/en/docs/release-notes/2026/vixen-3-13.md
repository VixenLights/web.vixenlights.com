---
title: "Vixen 3.13"
linkTitle: "Vixen 3.13"
weight: -313
description: Release notes for Vixen 3.13.
---

Vixen 3.13 was released on August 12, 2026. This release delivers a major platform modernization milestone alongside new sequencing, preview, export, and workflow improvements. It also includes a broad set of stability fixes across the sequencer, preview, fixtures, custom prop editing, marks, and effect editing.

## Highlights

Vixen 3.13 introduces the move to .NET 10 LTS, adds Universal Live Preview and Falcon Player direct upload, expands workflow support with Element Tags and the new State effect, and closes 116 Jira issues for this release.

## What's new

- **.NET 10 LTS platform upgrade** with supporting build and dependency updates, bringing the codebase onto the current long-term support stack.
- **Universal Live Preview** architecture with shared live preview messaging and refactored web server components. Used for visualizing State configuration in Display Setup.
- **Falcon Player direct upload** from the Export Wizard using REST-based integration.
- **[State effect]({{< ref "state" >}}) and State property workflow** including setup helpers and custom prop editor support.
- **[Element Tags]({{< ref "element-tags-sequencer" >}}) foundation** with core API, persistence, assignment services, and workflow integration.
- **Quality and reliability improvements** across preview rendering, fixture setup, timeline interaction, marks, text, gradients, curves, and export workflows.

## Release summary

| Area | Summary |
| --- | --- |
| Platform | Upgraded the application to .NET 10 LTS and modernized supporting infrastructure, including dependency refreshes, installer updates, build workflow alignment, and compatibility cleanup. |
| Preview | Added Universal Live Preview, transparent preview backgrounds, hidden locked preview elements, toolbar usability improvements, and multiple preview-related fixes. |
| Sequencing | Improved effect editing, drag-and-drop, cloning, waveform and ruler controls, mark handling, row navigation, and timeline interaction reliability. |
| Export and integration | Added direct upload to FPP, expanded export options, improved bulk export profile handling, and refined interoperability features such as Pangolin Beyond mark export. |
| Props and fixtures | Expanded fixture and state property support, improved fixture editor reliability, and strengthened custom prop editor persistence and import behavior. |
| Stability | Resolved 116 tracked issues, including crash fixes in video effects, fixture setup, OpenGL preview, alignment operations, and editor workflows. |

## Key enhancements

### Platform modernization

The Vixen codebase now targets **.NET 10 LTS**, representing one of the most significant under-the-hood updates in recent releases. This work includes runtime modernization, updated libraries, installer and build workflow improvements, binary serialization corrections, and cleanup of deprecated platform-specific patterns.

- [VIX-3781](https://vixenlights.atlassian.net/browse/VIX-3781) - Upgrade project to .NET 10 LTS
- [VIX-3832](https://vixenlights.atlassian.net/browse/VIX-3832) - Configure the build workflow to utilize a specific .NET SDK
- [VIX-3869](https://vixenlights.atlassian.net/browse/VIX-3869) - Correct binary serialization issues surfaced during the modernization effort
- [VIX-3966](https://vixenlights.atlassian.net/browse/VIX-3966) - Update dependencies to current versions
- [VIX-3932](https://vixenlights.atlassian.net/browse/VIX-3932) - Update libraries for security vulnerability

### Universal Live Preview

Live preview capabilities were reworked to support a more universal architecture. The release introduces shared live preview infrastructure, project-wide messaging updates, and web server refactoring intended to simplify future preview integrations and improve maintainability.

- [VIX-3925](https://vixenlights.atlassian.net/browse/VIX-3925) - Universal Live Preview: shared LivePreview module, Vixen.Messages broadcast project
- [VIX-3856](https://vixenlights.atlassian.net/browse/VIX-3856) - Convert deprecated web host usage in the web server project
- [VIX-3928](https://vixenlights.atlassian.net/browse/VIX-3928) - Add transparent background mode to Preview viewer
- [VIX-3768](https://vixenlights.atlassian.net/browse/VIX-3768) - Hide locked preview elements

### Falcon Player direct upload

Export workflows now support **direct upload to Falcon Player (FPP)**, reducing manual steps after sequence export and enabling a smoother handoff from sequencing to playback infrastructure.

- [VIX-3922](https://vixenlights.atlassian.net/browse/VIX-3922) - Add FPP Direct Upload capability to Export Wizard
- [VIX-3921](https://vixenlights.atlassian.net/browse/VIX-3921) - Add FPP REST API client module

### State property and State effect

Vixen 3.13 adds a new **State effect** and the supporting property model needed to build workflows around state-driven sequencing. This includes editor support, mapping helpers, and integration into the custom prop editor.

- [VIX-3924](https://vixenlights.atlassian.net/browse/VIX-3924) - Create the State Effect
- [VIX-3591](https://vixenlights.atlassian.net/browse/VIX-3591) - Create the State property and the mechanisms to apply it
- [VIX-3929](https://vixenlights.atlassian.net/browse/VIX-3929) - Add and edit the State property in the Custom Prop Editor
- [VIX-3942](https://vixenlights.atlassian.net/browse/VIX-3942) - Add element setup helper for the State property
- [VIX-3953](https://vixenlights.atlassian.net/browse/VIX-3953) - Fix save behavior when adding a new State in the mapping helper

### Element Tags foundation

This release introduces the foundational infrastructure for **Element Tags**, including core APIs, persistence, assignment services, and workflow-level integration. These changes establish a base for richer organization and targeting scenarios across display setup, preview setup, and sequencing.

- [VIX-3933](https://vixenlights.atlassian.net/browse/VIX-3933) - Element Tags core API and persistence
- [VIX-2690](https://vixenlights.atlassian.net/browse/VIX-2690) - [Element Tags]({{< ref "element-tags-sequencer" >}}) workflow across Display Setup, Preview Setup, and Sequencer
- [VIX-3931](https://vixenlights.atlassian.net/browse/VIX-3931) - Widen public APIs from ElementNode to IElementNode

## Notable user-facing improvements

- New waveform height lock option and ruler height lock option for more consistent timeline layouts.
- Improved mark handling, including scrolling while moving marks and better selection behavior.
- Support for cloning effects with constrained vertical-only movement using Ctrl+Shift drag.
- Move timeline cursor directly to the selected effect start.
- Additional target node selection and depth support for the [Wipe effect]({{< ref "wipe" >}}).
- Transparent preview background mode and improved preview setup responsiveness.
- Direct support improvements for custom props, fixture workflows, and xModel import scenarios.

## Stability and bug fixes

This release contains broad reliability work across the application. Particularly notable fixes include:

- [VIX-3981](https://vixenlights.atlassian.net/browse/VIX-3981) - Fixed a crash when a video effect is added without selecting a file and the sequencer is closed
- [VIX-3973](https://vixenlights.atlassian.net/browse/VIX-3973) - Fixed a crash when editing a fixture property row from Display Setup
- [VIX-3972](https://vixenlights.atlassian.net/browse/VIX-3972) - Corrected Fixture Wizard row selection issues
- [VIX-3910](https://vixenlights.atlassian.net/browse/VIX-3910) - Fixed broken OpenGL Preview behavior introduced during cleanup work
- [VIX-3923](https://vixenlights.atlassian.net/browse/VIX-3923) - Restored Preview configuration functionality in newer development builds
- [VIX-3939](https://vixenlights.atlassian.net/browse/VIX-3939) - Fixed crash when Shift-clicking row labels
- [VIX-3864](https://vixenlights.atlassian.net/browse/VIX-3864) - Fixed crash when copying a gradient onto Pinwheel
- [VIX-3853](https://vixenlights.atlassian.net/browse/VIX-3853) - Restored copying effects in development builds
- [VIX-3503](https://vixenlights.atlassian.net/browse/VIX-3503) - Fixed divide-by-zero fatal error scenario
- [VIX-3481](https://vixenlights.atlassian.net/browse/VIX-3481) - Fixed timeline alignment crash conditions

## Selected completed work by area

| Area | Representative issue | Description |
| --- | --- | --- |
| Sequencer workflow | [VIX-3940](https://vixenlights.atlassian.net/browse/VIX-3940) | Added Ctrl+Shift drag to clone effects with vertical-only movement. |
| Timeline usability | [VIX-3936](https://vixenlights.atlassian.net/browse/VIX-3936) | Moves the timeline cursor to the start of the selected effect. |
| Marks | [VIX-3944](https://vixenlights.atlassian.net/browse/VIX-3944) | Improved scrolling behavior while moving marks and mark labels. |
| Preview | [VIX-3928](https://vixenlights.atlassian.net/browse/VIX-3928) | Added transparent background mode to the Preview viewer. |
| Preview setup | [VIX-3962](https://vixenlights.atlassian.net/browse/VIX-3962) | Debounced Preview Setup zoom slider rendering for better responsiveness. |
| Effects | [VIX-3938](https://vixenlights.atlassian.net/browse/VIX-3938) | Added target node selection and depth support to the Wipe effect. |
| Audio visualization | [VIX-3948](https://vixenlights.atlassian.net/browse/VIX-3948) | Added waveform height lock option. |
| Display setup | [VIX-3285](https://vixenlights.atlassian.net/browse/VIX-3285) | Added full-screen display setup editor improvements. |
| Export | [VIX-3632](https://vixenlights.atlassian.net/browse/VIX-3632) | Added the ability to delete and rename bulk export profiles. |
| Integration | [VIX-3791](https://vixenlights.atlassian.net/browse/VIX-3791) | Added Pangolin Beyond mark export option. |

The 3.13 release contains work spanning new features, improvements, and defect resolution across preview architecture, FPP integration, state-based workflows, tagging infrastructure, export, marks, fixtures, custom props, effects, timeline interaction, installer modernization, dependency refreshes, and platform compatibility updates. For the authoritative full issue list, use the Jira release filter linked below.

## Upgrade guidance

- Review any environment or plugin dependencies that may be sensitive to the .NET 10 LTS runtime transition.
- Test export workflows, especially if adopting new FPP direct upload capabilities for the first time.
- For advanced display and prop setups, verify State property mappings and Element Tag workflows after upgrade.

## Links

- [Jira issues fixed in Vixen 3.13](https://vixenlights.atlassian.net/issues/?jql=project%20%3D%20VIX%20AND%20fixVersion%20%3D%20%223.13%22)
