---
# required metadata

title: "Delegate admin permissions to groups"
titleSuffix: Intune for Education
description: Learn how to manage roles for groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 9319be2e-cb7e-43c1-98fe-64281c8c09fd
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

# Delegate admin permissions to groups
You and your IT staff manage multiple groups of students, teachers, and administrators throughout your school.  

Unlike IT staff, admin groups only manage the groups you assign to them. When you give admin permissions to a group of qualified individuals, you help reduce the risk of unauthorized or accidental changes.  

## Group admin permissions 

Delegated group admins have permission to manage school devices and apps. Admin access lets them:

- View information about devices, users, and apps.
- Assign, create, delete, view, and update device and user settings.
- Assign, create, delete, view, and update apps.
- View reports.
- Take remote actions on devices, including resetting to factory settings, rebooting, locking an unlocked device, and forcing a sync.

> [!TIP]
> Modifying admin permissions is an advanced task. If you want to change the permissions or create a custom set of permissions, then you need to go to [the full management experience in Intune](group-admin-delegate.md#find-out-more). These permissions comprise the built-in School Administrator role in Intune. 

## Assign an admin group

1. From the Intune for Education dashboard, click **Groups**.
2. Choose a group. This group will be the one your admins manage.
3. Click the **Admins** tab > **Add Admins**.
4. Choose a group to give it admin permission to manage apps and settings.
5. Click **Choose group**.

## Remove an admin group
1. From the Intune for Education dashboard, click **Groups**.
2. Choose a group. This group will be the one your remove an admin group from managing.
3. Click the **Admins** tab.
4. Select one or more groups from the list of admins. Then click **Remove Admins**  

## Next steps

  - [Role-based administration control with Intune](https://docs.microsoft.com/intune/role-based-access-control)
