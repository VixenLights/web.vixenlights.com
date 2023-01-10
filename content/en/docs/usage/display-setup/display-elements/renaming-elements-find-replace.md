---
title: Renaming Elements by Find/Replace
author: Jeff
date: 2017-09-17T14:49:48+00:00
weight: 30
---
### Introduction

You may have element structures that were created with names that did not have the exact structure you wanted or have evolved over time and need some restructuring. The standard rename function has abilities to rename multiple items via a sequential template format.  At times, this may be too rigid for your needs and a simple find replace mechanism can better serve the purpose. An example is shown below where the paste as new function was used to duplicate a element group structure. The groupings themselves have elements that have been restructured out of a sequential naming structure. The intent here is to remove the - 2 on the end and change it from Snowflake 1 to Snowflake 5. This way the newly cloned element group will match the pattern of the original ones it was cloned from. See element [duplication]({{< ref duplicating-elements>}}) for additional details. Starting in 3.6 and above this can be done from the Display Setup or the Preview Setup forms.

![Snowflake Duplicate](/images/docs/usage/display-setup/display-elements/SnowFlakeDuplicate.png)

### Steps

1. Select a group of elements to Find/Replace naming patterns. They can be all together, or slected from multiple different levels. Select only the items you wish to act on.

2. Right click on the selected items and choose Find/Replace.

![Find Replace](/images/docs/usage/display-setup/display-elements/Find-Replace-214x300.png)

3. On the dialog box that appears you can create patterns of find and replace. Patterns can be chained to allow for multiple find replace operations in one pass without having to do the Find/Replace operation multiple times.

4. First we will create the pattern to rename Snowflake 1 to Snowflake 5. In the Find what text field we put Snowflake 1. In the Replace with text field we put Snowflake 5. You will notice the list at the left showing on the fly what will happen as you type the values in.

![Find Replace Dialog](/images/docs/usage/display-setup/display-elements/Find-Replace-Dialog-1.png)

5. Next we also want to remove the - 2 on the end. So we click the green + button to add a new pattern. This new Find/Replace will occur on the result of the previous pattern. We enter a the - 2 in the find what. Notice we enter a blank space in front because we also want to remove the blank that is there. - 2. Because we want to replace that with nothing, we leave the replace with text field empty. The list on the right updates to reflect the result of all our changes.

![Find Replace Dialog](/images/docs/usage/display-setup/display-elements/Find-Replace-Dialog.png)

6. Now that the list on the right reflects what we want the elements to look like, we can click the ok button and the changes will be applied.</p>
