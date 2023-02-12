---
title: Select Profile
date: 2017-01-05
weight: 10
description: Information about selecting or creating a DMX intelligent fixture profile.
aliases: [/vixen-3-documentation/setup-configuration/setup-display-elements/intelligent-fixture-wizard/select-profile/]
---

---

![Select Profile](/images/docs/usage/display-setup/display-elements/intelligent-fixture-wizard/SelectProfile.png)


---

### Select Profile Options

* **Select Existing Profile** - If you have already created a Profile for your fixture you could select it here.  The drop down shows all fixtures installed into the active Vixen profile.  The fixture profiles are stored within the Vixen profile.
Note in the future users may be able to download fixture profiles from the Vixen website that other users have submitted.

* **Create New Profile** - The default is to create a new fixture profile.  The fixture profiles are stored within your overall Vixen profile.

---

### Profile Properties

* **Profile Name** - Name of the intelligent fixture profile.  For new fixture enter a unique name.  This name is used as the fixture profile filename.

* **Manufacturer** - Optional name of the manufacturer of the fixture hardware.

* **Created By** - This read-only field is determined by the Windows login name.

* **Revision** - Field for keeping track of updates to the profile definition.  Refer to Persistance Note below for implications of updating a profile.
               If the profile is being updated consider incrementing the **Revision** number.

---

### Persistance Note

If the Profile Name is changed it is effectively as 'Save As'' like operation as the existing profile is not modified.
If anything is changed in a profile, only newly created fixtures will receive the changes.
Existing fixtures are NOT impacted by the changes and if desired will need to be updated via their _**Intelligent Fixture**_ property.

---

Select the _**Next**_ button to continue to configure your intelligent fixture.

### Video Tutorials

{{< youtube 5sCJ_iqTQQ4>}}

---

{{< youtube Q9K5AtgapZo>}}

---

