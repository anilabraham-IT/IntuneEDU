---
# required metadata

title: Assign group admins  
titleSuffix: Intune for Education
description: Learn how to assign admin permissions to groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 01/07/2020
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
#ms.reviewer: elcox
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Assign admin permissions

Give admin permissions to a group of qualified individuals at your school to help reduce the risk of unauthorized or accidental changes in Intune for Education. People assigned as admins can sign in to Intune for Education and manage user and device groups. They can only see and make changes to the groups you assign them.  

Group admins can:  

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

## Assign group admins    
There are two ways to assign group admins in Intune for Education:

* Select a device or user group, and then add new group members as admins. 
* Select an admin group, and then add a device or user group for the admins to manage.  

### Add group members as admins:  
Complete these steps to add admins to a device or user group.  

1. From the dashboard, select **Groups**.
2. Choose a group.   
3. Select the **Admins** tab > **Admins of this group**.  
4. Select **Add admins**.
5. Choose a group. Members of this group will get permission to view and manage devices and apps assigned to the group you chose in step 2.  
6. Select **Choose group to add the group members as admins**.   

### Add a group to manage  
Complete these steps to assign a device or user group to a group of admins.  

1. Choose a group.  
2. Select the **Admins** tab > **Managed by this group**.  
3. Select **Add a group to manage**.  
[SCREENSHOT OF THIS IN THE UX – PENDING]  
4. Choose a group. The devices and apps assigned to this group will be managed by the group you chose in step 1. 
5. Select **Choose group**.  

## Remove admin permissions  

To remove admin permissions from people in your school, you can either:  
* Select a device or user group and remove the associated admins.  
* Select an admin group and remove an associated device or user group.  

### Remove admins  
Complete these steps to remove a group of admins from a device or user group.  
1. From the dashboard, select **Groups**.
2. Choose a group. 
3. Select the **Admins** tab > **Admins for this group**.
4. Choose one or more groups. These groups will no longer have permission to view or manage the devices and apps that belong to the group you chose in step 2.  
5. Select **Remove admins**.  

### Remove device or user group  
Complete these steps to remove a device or user group from a group of admins. 
1. From the dashboard, select **Groups**.  
2. Choose a group.  
3. Select the **Admins** tab > **Managed by this group**.
4. Choose one or more groups. These groups will no longer have permission to view or manage the devices and apps that belong to the group you chose in step 2.  
5. Select **Remove group**.  

## Restrict iOS VPP token access
If you're in a school district that has iOS devices at multiple locations, it’s a good idea to restrict VPP token access to select admins. These tokens will only be accessible to admins if the token has been added to their group's restricted token list.       

1. From the dashboard, select **Groups**.  
2. Choose a group.   
3. Select the **Admins** tab. To view admins of the current group, select **Admins of this group**. To view groups that this group can manage, select **Managed by this group**.  
4. Choose an admin group from the list. Two additional lists appear:  
    * The top list shows all restricted VPP tokens. These tokens and their associated apps can only be accessed by the selected group.  
    * The bottom list shows all unrestricted VPP tokens. These tokens and their associated apps can be accessed by anyone with admin permissions.  
1. To add a token to the group's restricted list you can either:  
    * Use the search bar to find a token. Select the token from the search results.  
    * Choose a token from the unrestricted list and then select **Restrict to these admins**.  
1. Select **Save**.   

Now that the token is a part of the admins' restricted list, only these admins can see and manage the token and its associated apps. Repeat these steps for each group to restrict all VPP tokens to their respective admins.  