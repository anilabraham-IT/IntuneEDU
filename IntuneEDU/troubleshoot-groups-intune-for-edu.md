---
# required metadata

title: Create groups in Intune for Education
titleSuffix: Intune for Education
description: Learn how to manage groups of devices with Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: doueby
ms.date: 10/08/2018
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

This article answers common questions about creating and editing groups in Intune for Education.

## Why can't I edit the default groups?

At the time that you create your account, Intune for Education creates a set of default, tenant-level groups. These groups&ndash;**All Users** and **All Devices**&ndash;can't be changed. After you import your school and teacher records from School Data Sync, Intune creates additional groups, called **All Teachers** and **All Students**. These groups can't be changed either.

In rare situations, you might end up with the same subgroup underneath two groups. If this problem occurs, move one of the top-level groups above the subgroup.

## Why can't I edit dynamic groups?

Intune for Education lets you pick from a subset of dynamic attributes in Intune's full management portal. If the attribute that you want to edit is not visible in the Intune for Education portal, you must edit it in Intune in the Azure portal or Azure Active Directory.

## Why can't I edit a specific group?  

Intune for Education is designed to be an easy way to manage devices in your schools. It uses [Intune in the Azure portal](https://docs.microsoft.com/intune/what-is-intune)&ndash;an enterprise product&ndash;to manage apps and groups. Certain admins in your organization have permission to use both Intune in the Azure portal and Intune for Education to create special groups. If you can't edit a group, it's likely that it was created in Intune in the Azure portal, and you don't have permissions to modify the group.  
