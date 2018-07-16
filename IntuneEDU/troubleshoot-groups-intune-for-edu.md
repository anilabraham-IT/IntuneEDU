---
# required metadata

title: Create groups in Intune for Education
titleSuffix: Intune for Education
description: Learn how to manage groups of devices with Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: doueby
ms.date: 07/23/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 4b570196-a640-4d13-8e01-8e8553ce1468
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

# Troubleshooting group actions

The article provides answers to questions about creating and editing groups in Intune for Education.

## Why can't I edit the default groups?

Intune for Education creates a set of default, tenant-level groups when your school's account is created. These groups, **All Users** and **All Devices**, cannot be changed. The **All Teachers** and **All Students** groups are created after School Data Sync has imported student and teacher data into Intune for Education, and cannot be changed either.

In rare situations, you may end up with the same subgroup underneath two groups. If this problem occurs, move one of the top-level groups above the subgroup.

## Why can't I edit dynamic groups?

Intune for Education lets your pick from a subset of the dynamic attributes available in Intune's full management portal. If the attribute that you want to edit is not visible in the Intune for Education portal, you must edit it in Intune in the Azure Portal or Azure Active Directory.

## Why can't I edit a specific group?  

Intune for Education is designed to be an easy way to manage devices in your schools. It uses [Intune in the Azure portal](https://docs.microsoft.com/intune/what-is-intune), an enterprise product, to manage apps and groups. Certain admins in your organization have permission to use both Intune in the Azure portal and Intune for Education to create special groups. If you can't edit a group, it's likely that it was created in Intune in the Azure portal, and you don't have permissions to modify the group.

## Next steps

- [Find out more about the full groups management experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
