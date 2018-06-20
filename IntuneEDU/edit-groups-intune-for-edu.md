---
# required metadata

title: Edit groups in Intune for Education
titleSuffix: Intune for Education
description: Learn how to edit existing user and device groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/20/2018
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

# Edit existing groups

This article describes how to change the following group attributes from the Intune for Education portal > **Groups** page:

* Group name
* Group membership
* List location
* Group rules 

## Edit group name   
Change the name of an existing group.
1. Click the group you want to edit in your **Groups list**.
2. Click **Rename**.
3. Enter a new name in **Group name**.
4. Click **OK**.

## Manually assign members  
Follow this procedure to add or remove users and devices to an existing assigned group.

If you add or remove a member of a group, the member, whether it is a device or user, may experience a change in access or permissions.

The instructions below detail how to edit *user* membership. These steps can also be followed to edit membership for device groups.

1. Go to **Groups** and select the group you want to assign users to. 
2. Click *Edit user membership**.
3. To assign users:
    a. Select one or more members of **All other users**. 
    b. Click **Add users**. 
4. To unassign users  
    a. Select one or more members of **Users in group**.
    b. Click **Remove users**.
5. Click **OK**.

![Editing devices in a group](./media/groups-008-edit-group-membership.png)


## Edit group rules  
Adjust dynamic group rules to accommodate new devices, locations, or school years.

Editing existing rules may remove devices or users who were previously members of the group. Edits may cause them to experience a change in permissions or access. 

1. Go to **Groups** and select the group you want to edit.
2. Click *Edit group rules**.
3. Make changes to the rules. 
4. Click **Save changes**.  

## Move a group  

Move a group up or down within your existing group list in Intune for Education. If you distribute settings differently throughout your group list, moving a group higher or lower on the list changes its scope of settings.

Generally, the higher the position of the group, such as at parent level, the broader its settings.

  ![Move group buttons encircled in red](./media/groups-010-move-groups.png)

1. From the **Groups** list, select the group that you want to move.
3. Click **Move Group**.
4. Select or search for the location where you want to move the group. 
5.	Click **OK**.

## Find out more  

- [Find out more about the full groups management experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
