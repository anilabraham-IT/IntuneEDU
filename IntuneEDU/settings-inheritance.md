---
# required metadata

title: "What is settings inheritance?"
titleSuffix: Intune for Education
description: Learn how to manage settings for groups of devices with Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 09/26/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.subservice: education
ms.technology:
ms.assetid: 4b69b884-bed9-43f4-8507-c802228a8804
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: rashok
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# What is settings inheritance?

Settings are applied to groups. Since groups are set up as hierarchies, with one group above another, all settings applied to a group are inherited by its subgroups. Subgroups automatically take on the changes you make to the group above it. This action is called _inheritance_. Settings inheritance is helpful when you want to apply settings to large groups of users and devices.  


  ![A tree of groups of and subgroups.](./media/groups-002-inheritance.png)  


## Configure subgroups individually  

To override recently inherited settings, go directly to the subgroup. Configure it individually by removing or adding settings. Then save your changes.

## Settings in conflict  

If you apply conflicting settings to the same group, Intune will analyze each one individually. Intune always chooses the settings that, with certainty, complies with school policies.

In other cases, when Intune can't resolve the conflict, you should review the [settings conflict](what-are-reports.md) report.

### Example of inheritance conflict  

As an example, consider the subgroup, *12th Grade AP Computer Science*. The subgroup falls under the parent group, *12th grade*. You assign a strict security scanning requirement to all files and apps downloaded devices in the *12th grade* group.

However, you know that for an upcoming assignment, *12th Grade AP Computer Science* must download JavaScript files that don't need to be scanned. If you don't override settings inheritance, the more restrictive *Twelfth Grade* setting will be applied to the users in *Twelfth Grade AP Computer Science*.

## Settings error report

If a setting can't be resolved, it will appear in the Settings error report. For more information about reports, see [View and download reports](what-are-reports.md).  

## Next steps  
Find out more about the [full groups experience in Intune](https://docs.microsoft.com/mem/intune/fundamentals/groups-add).
