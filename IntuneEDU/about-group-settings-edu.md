---
# required metadata

title: What are group settings?
titleSuffix: Intune for Education
description: Learn how to manage settings through Intune for Education policies.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 91d004c0-8d06-4307-8868-46ac7b119101
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

# What are group settings?

Configure group settings to manage how students, teachers, and devices work in your school.

When you assign settings to users in a group, the settings stick with the users, no matter what devices they use. When you assign settings to devices in a group, the settings stick with the devices, no matter who uses them.  

Settings are applied to groups. Since groups are set up as hierarchies, with one group above another, any [settings applied to a group are inherited by all of its subgroups](settings-inheritance.md). This makes it easier to apply settings to large groups of users, apps, and devices.  

There are two ways to manage group settings in Intune for Education:  

* __Express configuration__: Configure a selection of the most commonly used school settings. [Express configuration](Express-configuration-intune-edu.md) is a walkthrough-style setup that helps you select and assign group settings quickly. Settings are preconfigured to Microsoft-recommended values but can be changed to fit your school's policies. 

* __Groups__: Configure all settings for any group of devices or users. In the **Groups** tab you'll see the full list of settings available in the portal. See are the settings available for [Windows](all-edu-settings-windows.md) and for [iOS](all-edu-settings-ios.md) groups.  

## Configure express configuration settings  

Express configuration can be used when you're just getting started in the portal, or when you've been using it for a while and want to make quick changes. For a detailed look at the express configuration steps, see [Express configuration in Intune for Education](Express-configuration-intune-edu.md).

  ![Express Configuration settings fix](./media/express-config-006-choose-settings.png)  

## Configure settings in Groups

The following steps describe how to assign settings from the **Groups** page in Intune for Education. From this page, you'll see the complete list of device restrictions and features.  
1. From the Intune for Education dashboard, click **Groups**.
2. Select the group you want to configure.
3. Click **Settings** to view the full list of available settings.
4. Expand each category to modify individual settings for the selected group.
5. When you're done, click **Save**. Settings are automatically updated on all devices in the group.  

## Can I ever have settings that don't work together?

It is possible for incompatible settings to be applied to the same group. These inconsistences result in errors, when a user or device is being set up with different settings in multiple places. This happens as a result of the user or device being a member of multiple groups.

For example, Esperanza is a member of the *6th Grade* group and is also a member of group called *Earth Science*. If you configure a homepage setting and assign to *6th Grade*, and you configure a different homepage setting and assign it to *Earth Science*, she now has two conflicting homepage settings assigned to her user. That results in inconsistent settings assignment leading to an error. You can find which devices and users have settings errors using the [settings errors report](what-are-reports.md).

## Next steps
[Create user and device groups](what-are-groups.md) in Intune for Education so that you can start configuring their settings.  

[Find out more about how to protect apps and data with the full management experience in Intune](https://docs.microsoft.com/intune/deploy-use/protect-apps-and-data-with-microsoft-intune)
