---
# required metadata

title: Create groups in Intune for Education
titleSuffix: Intune for Education
description: Learn how to manage groups and subgroups of devices in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: doueby
ms.date: 07/23/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.subservice: education
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

# Create groups  

Create groups to manage users, apps, and devices that have similar management needs. Groups allow you to manage, assign, and apply changes in bulk, reducing the time you'd spend individually managing and troubleshooting devices. 

## Default groups  
Out-of-the-box, Intune for Education comes with default groups that enable you to manage:  
* All devices
* All users

Two additional default groups are created if you used School Data Sync to import your school records. They enable you to manage:  
* All teachers
* All students

These default groups represent the broadest categories of users and devices in your school and can't be changed or removed.

## Custom groups  

Apply specific or scenario-based configurations to custom-created groups. If you have both Windows 10 and iOS devices in your school, create groups, such as all iPads and all Windows 10 PCs. This way, you'll be able to more easily recognize groups and distribute settings. 

You can also assign apps and settings to specific groups of students. For example, an 8th grade curriculum may require different apps than a 6th grade curriculum. You can create two, grade-specific groups and assign apps and settings that are appropriate for each set of students.  
## Group types  

There are two types of groups that you can use to organize users and devices in Intune for Education: assigned groups and dynamic groups.

### Assigned groups  

Assigned groups are used when you want to manually add users or devices to a group.  Think of it like putting a filing system together: you'll file specific papers into a specific folder using your own logic or method of grouping. When you need those papers, you'll know the exact folder to go to. 

Similarly, you can create folders within folders, or *subgroups*, to further organize a larger group into a manageable size.

To learn how to manually assign or remove members, see [Edit groups](edit-groups-intune-for-edu.md).


### Dynamic groups  
Dynamic groups reference rules that you create to assign students or devices to groups. The criteria for rules is specified during initial group creation, and can be edited after a group is created.

For example, you can create a group specific to students graduating from Contoso High at the end of the 2019 school year. Rather than go through and assign each student manually, Intune for Education would filter the students into the group based on school and graduation date.

If a student within the group transfers out of Contoso High and into another school in your district, you would not be able to manually remove them from a dynamic group. Instead, you would need to update the student's school name so that Intune knows that they know longer meet the group criteria for membership.

Since dynamic groups can only contain what their rules define, you cannot create subgroups under them.

To learn how to edit group rules, see [Edit groups](edit-groups-intune-for-edu.md).

> [!TIP]
> Use the dynamic rules to filter through groups of similarly-named or recently onboarded groups of devices, such as *DeviceType_School_Grade_0001*. Dynamic groups are ideal for managing large groups of devices or users in large school districts. They reduce the time and costs required to manually go through a school's inventory or headcount.  


## Plan your groups
To get started, plan out the settings and apps required for your school district, students, teachers, and devices. Settings are assigned to groups, and some groups will require specific settings and apps.   

For example:  
* For all devices, block apps from using location services. 
* For AP computer science, assign students apps to edit code.
* For 12th grade history students, enable web browsing so they can access academic articles.
* For photography students, enable device camera.


## Create a group  
Groups must be created one a time. During setup, you'll select to create a group for either users or for devices.

1. From the Intune for Education dashboard, click **Groups** > **Create group**.
2. Enter a descriptive group name.
3. Select a group type. For more details about assigned and dynamic groups see [Group types](## Group types)   
    a. Assigned: Manually add and remove users and device in these groups. If you select this option, go to step 5.
    b. Dynamic: Rules are implemented to automatically add and remove users and devices. If you select this option, go to step 4.
4. Select to manage devices or students.
    a. Devices: If you select this, a naming rule appears. Create a rule to automatically assign devices that start or contain the text you input. As you type, a preview of members will populate at the bottom of the page.
    b. Students: If you select Students, a location and identification rule appears. Create a rule to automatically assign students that go to a specific school in your tenant. Then select to group students by grade or graduation year. After you input all fields, a preview of members will populate at the bottom of the page.
5. At the bottom of the page, click **Create group**.

## Create a subgroup  
Groups are set up in Intune for Education as hierarchies. The parent group is the top of the hierarchy, and [any settings applied to this group are inherited by the groups under it](settings-inheritance.md). This concept is known as *settings inheritance*.  Setting inheritance makes it easier to apply settings to a large group of users and devices. 

Subgroups can only be created *under* assigned groups. 

 ![The create subgroup page, with the two locations for subgroup creation — at the top of the group name and the sidebar — encircled in red](./media/groups-007-create-subgroup.png)

1. Go to **Groups** and choose a group. This group will be the parent to your subgroup.
2. Click **Create sub group**.
3. Enter the **Group name**. 
4. Select your group type. For more details about group types, see the steps for [Create a group](#create-a-group) above.
5. Click **Create group**.  

## Next steps 
[Delegate permission](group-admin-delegate.md) to allow admin groups to manage parent level groups and subgroups.  

[Learn about the full](https://docs.microsoft.com/mem/intune/fundamentals/groups-add) groups management experience in Intune.
