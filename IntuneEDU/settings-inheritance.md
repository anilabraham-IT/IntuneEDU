---
# required metadata

title: "What is settings inheritance?"
titleSuffix: Intune for Education
description: Learn how to manage settings for groups of devices with Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 01/17/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
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

Settings are applied to groups. Since groups are set up as hierarchies, with one group above another, any settings applied to a group are inherited by all of its subgroups. This makes it easier to apply settings to large groups of users, apps, and devices.

  ![A tree of groups of and subgroups.](./media/groups-002-inheritance.png)

Subgroups automatically take on the changes you make to the group above it. This is called _inheritance_.

## Configure subgroups individually 

Subgroups can be configured individually, even if they are inheriting settings from the group above them. Override inherited settings by configuring the settings that you need within the specific group, and then saving them.

## Settings in conflict

When multiple settings have been applied to the same group, each setting is analyzed individually by Intune for Education. Settings that force users to take action to make their devices comply with your settings will always take precedence over other settings.

Consider a subgroup, *Twelfth Grade AP Computer Science*, to the group *Twelfth Grade*. You know that the AP computer science class will need to download some JavaScript files that do not need security scanning, but you want to make sure that the whole grade does not try to do the same. If you do not override settings inheritance, the more restrictive *Twelfth Grade* setting will be applied to the users in *Twelfth Grade AP Computer Science*.

If a setting cannot be resolved, it will appear in the Settings error report. See [View and download reports](what-are-reports.md) for more information about reports in Intune for Education.

## Find out more

  - [Find out more about the full groups experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
