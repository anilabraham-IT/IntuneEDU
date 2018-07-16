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

# Microsoft School Data Sync and Intune for Education

Microsoft School Data Sync (SDS) is a free service in Office 365 Education that imports school records from your existing Student Information System (SIS). It creates online classrooms and groups for Microsoft Temas, Intune for Education, and third-party applications.  

Go to the School Data Sync documentation to [learn how to deploy SDS](https://support.office.com/article/Overview-of-School-Data-Sync-and-Classroom-f3d1147b-4ade-4905-8518-508e729f2e91). 

## Create groups from school roster
SDS creates copies of the information from your SIS, and stores it in Azure Active Directory (Azure AD). SDS creates two groups in Intune for Education to which you can apply settings and apps:

* All Students
* All Teachers

For more information about creating groups in Intune for Education, see [Create groups](what-are-groups.md).  

## Set up dynamic group properties
When importing student information from your SIS into Intune for Education with School Data Sync, include the properties __Grade__ and __Graduation Year__. These properties are necessary to create [dynamic group](what-are-groups.md#dynamic-groups) rules for students in the Intune for Education portal. 

Properties are configured from the SDS app, and are found in  __Student options__ > __Select student properties__.

## What is Azure AD?
Azure AD is a Microsoft management system that integrates with Intune and helps organize students and devices. It lets you create groups out of your students and teachers, such as *4th period Biology* or *Contoso District teachers*. Groups are necessary to assign and distribute user or device-specific apps, settings, and restrictions.

## Next steps  
[Find out more about Microsoft School Data Sync](https://sds.microsoft.com). After your student and teacher information is synced with Intune for Education, get started with express configuration for [Windows](edu-express-config-settings-windows.md) or [iOS](edu-express-config-settings-ios.md) devices.
