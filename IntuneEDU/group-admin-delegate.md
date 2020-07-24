---
# required metadata

title: "Delegate admin permissions to groups"
titleSuffix: Intune for Education
description: Learn how to manage roles for groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 11/22/2019
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.subservice: education
ms.technology:
ms.assetid: 9319be2e-cb7e-43c1-98fe-64281c8c09fd
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: elcox
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Delegate admin permissions to groups
You and your IT staff manage multiple groups of students, teachers, and administrators throughout your school.  

Unlike IT staff, admin groups only manage the groups you assign to them. When you give admin permissions to a group of qualified individuals, you help reduce the risk of unauthorized or accidental changes.  

## Group admin permissions 

Group admins are assigned in Intune for Education and have permission to manage school devices and apps. Group admins can:  

- View information about devices, users, and apps.
- Assign, create, delete, view, and update device and user settings.
- Assign, create, delete, view, and update apps.
- View reports.
- Take remote actions on devices, including resetting to factory settings, rebooting, locking an unlocked device, and forcing a sync.  
- Create, delete, view, and update the iOS MDM Push Certificate, iOS MDM server tokens, and iOS VPP tokens.   
- Assign and delete an Apple user-initiated enrollment profile.  
- Assign and delete Windows Autopilot deployment profiles.  
- Initiate a sync on devices registered with the Windows Autopilot service.   
- Assign users to devices registered with the Windows Autopilot service.  
- Delete devices registered with the Windows Autopilot service.  

> [!TIP]
> Modifying admin permissions is an advanced task. If you want to change the permissions or create a custom set of permissions, then you need to go to [the full management experience in Intune](https://docs.microsoft.com/intune/role-based-access-control). These permissions comprise the built-in School Administrator role in Intune. 

## Assign an admin group

1. From the Intune for Education dashboard, click **Groups**.
2. Choose a group. This group will be the one your admins manage.
3. Click the **Admins** tab > **Add Admins**.
4. Choose a group to give it admin permission to manage apps and settings.
5. Click **Choose group**.

## Remove an admin group
1. From the Intune for Education dashboard, click **Groups**.
2. Choose a group. This group will be the one you remove an admin group from managing.
3. Click the **Admins** tab.
4. Select one or more groups from the list of admins. Then click **Remove Admins**.  
