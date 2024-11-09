---
title: Issue Management
author: Vixen Team
weight: 40
description: This section covers managing issues in JIRA.
---

### Overview

We use JIRA to track feature requests, bug reports, improvements, and other development-related work for the Vixen application.  This page will explain the structure and layout of some of the JIRA tickets, the processes we go through when working on them, and any other related notes. For documentation issues, see [Contributing to Documentation][3].

The [JIRA bug tracker][1] can be found here. We are currently utilizing the cloud version of JIRA, so the link here will redirect you to the Atlassian location for our cloud instance. If you have a question that is not answered on this page, please ask!

The purpose of JIRA is to keep track of any outstanding issues relating to Vixen.  These might be bugs with existing functionality, or requests for new features (or improvements to existing ones).  Please try and make sure that we track ALL work that needs to be done in JIRA, as it lets us keep a record of it.  So often there is a bug report posted on the DIYC forum, or the Dev mailing list, which goes unanswered (or unsolved), and gets forgotten.  Please try and make new tickets for everything; they're easy to close if needed!

### JIRA Tickets

JIRA tickets have a number of fields that can be used to help describe and categorize an issue.  Some are mandatory, some are useful, and some not as much. When creating a ticket, ensure you complete the items in the following list with an asterisk (<span style="color: #ff6600;">*</span>).

* **Issue Type** (<span style="color: #ff6600;">*</span>)  Can be one of five values:
  * **Epic**  To track larger projects that are underway. Do not use.
  * **Bug**  Something in the software does not work as described or expected.
  * **Improvement**  An existing feature could be improved with this work.
  * **New Feature**  This does not exist in the software, and would improve it.
  * **Task**  Used to track miscellaneous development work, not strictly tied to the software functionality (eg. code cleanup, research, etc.)
* **Summary** (<span style="color: #ff6600;">*</span>)  One-line title of the issue.
* **Priority:**  Defaults to _Major_, not often changed. Can change if it&#8217;s particularly important or not.
* **Component/s** (<span style="color: #ff6600;">*</span>) One or more areas of the software that this relates to. Ask for new ones if needed.
* **Affects Version**  Only used when reporting a bug.
* **Fix Version** This should be added when the code is merged and will be included in the next version.
* **Assignee/Reporter** Who is working on it, and who reported it.
* **Description/Attachements** (<span style="color: #ff6600;">*</span>)  Include as much detail about the problem here. If needed, attach config files, sequences, logs, etc.
* **Task Group**  We tried to use this to track a rough timeframe of when work would be done. Finding it too hard to predict, so we've stopped using it.
* **Epic Link**  Which _Project_ of work this falls under, if any. Leave empty unless you're sure of what it should be.

### Epic/Project Tickets

The Epic tickets are used to track large chunks of work, as there may be a number of bugs or requested improvements related to one particular field. For example, there's many improvements to the sequencer to be considered when we revamp the sequencer, so these are all grouped together to make it easy to track them, review them, etc.

We have a number of Epics are the moment. Some are just to collate small related problems, and others are to section out large chunks of work that have many facets that need considering.  These should help to make it easier to track work on a single _Topic_. Since we often get developers that are interested in one particular area, this will make it easier to point them at a single point to manage the work being done.

### Lifecycle of a Ticket

The lifecycle of a Vixen ticket can be seen below. A full explanation of the process follows.

Note that to be able to do a some of these functions, you need to have appropriate permissions. Most active developers will need the **JIRA Developer** role. If you are unable to take tickets or progress them through the workflow, ask the dev group, and we can change your permissions.

1. A ticket is created (eg. a user reports a bug, requests a feature, or a developer makes a ticket for work they have been doing). It may be assigned to someone specific if relevant.
2. Someone takes it, and starts working on it (even if it's just reviewing it, or reproducing the issue). They assign it to themselves, and change it to **In Progress**.  This helps prevent multiple people duplicating work. If you are doing work on a Git branch, the name of the branch should be the ticket number (ex VIX-2100) and all commits should start with the JIRA issue number.
3. They finish their work on it. If it has not been fixed or completed, leave a comment explaining what has happened with it, and put it back to **Open**. If work has finished on it, you next step is to create a PR request in GIT and the JIRA ticket transitions will occur automatically from there. The developer does not need to manually move the ticket to **Ready to Merge**.
4. The maintainer reviews it. If it's OK, they will merge it into master, and it will progress into **Merged / Building** in JIRA. If there's some concerns about it, the maintainer comments in Github or in the issue itself. It then goes back to the developer to review, fix, etc. (go to step #3).
5. Once it is merged, a development build will automatically be created and uploaded to the dev builds area of the website. Here it can be reviewed by other users or developers. The ticket will be closed with a field indicating the build number the resolution is contained in. If any issues are found, the ticket can be reopened, or a new bug filed that references the original ticket. If it is reopened go to step #3.
6. The ticket stays **Resolved** for a while, until we do a public release. At this point, all **Resolved** tickets are used to build up release notes (to track what work as been done), they can be edited to include what version they have been fixed in, etc.  Once the release is public, those tickets will be marked with the release build number.

Note that this process does not have any documentation steps integrated into it. If the work you do on a ticket involves updating the application documentation. i.e this site, then you should create a cooresponding issue in the Github issues for this site and document the needed changes. You can then make those changes or ensure they are documented so that someone else can.

### Ticket Searches

There's a number of searches we have made that can be handy:

[All **Open** tickets by number][2]

[1]: http://bugs.vixenlights.com
[2]: http://bugs.vixenlights.com/issues/?filter=10000
[3]: {{< ref "contribute-docs#creating-an-issue" >}}
