---
# required metadata

title: Import school records with School Data Sync
titleSuffix: Intune for Education
description: Use School Data Sync to import school groups and people into Azure AD.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 08/11/2017
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: f9cb6daf-a789-427b-bbfd-fa0a3d36e01f
searchScope:
 - IntuneEDU

 # optional metadata

 #ROBOTS:
 #audience:
 #ms.devlang:
 #ms.reviewer: travisj
 #ms.suite: ems
 #ms.tgt_pltfrm:
 #ms.custom: intune-education

---

# What is School Data Sync?

Use Microsoft School Data Sync (SDS) to import school records from an existing Student Information System (SIS).[Learn how to deploy SDS](https://support.office.com/article/Overview-of-School-Data-Sync-and-Classroom-f3d1147b-4ade-4905-8518-508e729f2e91).

SDS creates copies of the information from your SIS, and stores it in Azure Active Directory (AD). Azure AD is a Microsoft management system that integrates with Intune and helps organize students and devices. It lets you create groups out of your students and teachers--such as 4th period Biology or Contoso District teachers. Groups are neccessary to assign and distribute user or device-specific apps, settings, and restrictions.

When importing student information from your SIS into Intune for Education with School Data Sync, make sure that you include __Grade__ and __Graduation Year__ if you intend to make [dynamic groups](what-are-groups.md#managing-groups-and-subgroups) with those properties. This is under __Student options__ > __Select student properties__. You use this information to create a profile.  

## Find out more

- [Find out more about Microsoft School Data Sync](https://sds.microsoft.com)
