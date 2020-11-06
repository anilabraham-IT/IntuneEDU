---
# required metadata

title: Assign group admins  
titleSuffix: Intune for Education
description: Learn how to assign admin permissions to groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 11/05/2020
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

People assigned as admins in Intune for Education can manage user and device groups. It's important to only give these permissions to qualified individuals, to reduce the risk of unauthorized or accidental changes in Intune for Education. Users with admin permissions can only see and make changes to the groups you assign them.  

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


### Building custom roles  
All the permissions needed to use Intune for Education are included in the built-in School Admin role. If you want to build a custom role that allows access to Intune for Education, you can duplicate the built-in School Admin role and add/remove permissions to create the role you want.

To build a custom set of admin permissions, switch to the full management experience in Microsoft Intune and go to **Tenant administration** > **Roles**. For more information about role-based access, see [Role-based access control (RBAC) with Microsoft Intune](/mem/intune/fundamentals/role-based-access-control).  

## Assign group admins    
There are two ways to assign group admins in Intune for Education:

* Select a device or user group, and then add new group members as admins. 
* Select an admin group, and then add a device or user group for the admins to manage.  

### Add group members as admins   
Complete these steps to add admins to a device or user group.  

1. From the dashboard, select **Groups**.
2. Choose a group.   
3. Go to **Admins** > **Admins of this group**.  
4. Select **Add admins**.
5. Choose a group. 
6. Select **Add groups**.   

### Add a group to manage  
Complete these steps to assign a device or user group to a group of admins.  

1. Choose a group.  
2. Go to **Admins** > **Managed by this group**.  
3. Select **Add groups to manage**.  
4. Choose a group.  
5. Select **Add groups**.  

## Remove admin permissions  

To remove admin permissions from people in your school, you can either:  
* Select a device or user group and remove the associated admins.  
* Select an admin group and remove an associated device or user group.  

### Remove admins  
Complete these steps to remove a group of admins from a device or user group.   
1. From the dashboard, select **Groups**.
2. Choose a group. 
3. Go to **Admins** > **Admins of this group**.
4. Select one or more groups.   
5. Select **Remove admins**.  

### Remove device or user group  
Complete these steps to remove a device or user group from a group of admins. 
1. From the dashboard, select **Groups**.  
2. Choose a group.  
3. Go to **Admins** > **Managed by this group**.
4. Select one or more groups.  
5. Select **Remove groups**.  

## Restrict iOS VPP token access
If you're in a school district that has iOS devices at multiple locations, it’s a good idea to restrict VPP token access to select admins. These tokens will only be accessible to admins if the token has been added to their group's restricted token list.       

1. From the dashboard, select **Groups**.  
2. Choose a group.   
3. To view admins of the current group, select **Admins of this group**. To view groups that this group can manage, select **Managed by this group**.  
4. Select an admin group > the **More** ellipses icon > **Restrict admin access**. Two additional lists appear:  
    * The top list shows all restricted VPP tokens. These tokens and their associated apps can only be accessed by the selected group.  
    * The bottom list shows all unrestricted VPP tokens. These tokens and their associated apps can be accessed by anyone with admin permissions.  
5. To add a token to the group's restricted list you can either:  
    * Use the search bar to find a token. Select the token from the search results.  
    * Find a token in the unrestricted list and select **Restrict to these admins**.  
6. Select **Save**.   

Now that the token is a part of the admins' restricted list, only these admins can see and manage the token and its associated apps. Repeat these steps for each group to restrict all VPP tokens to their respective admins.  
