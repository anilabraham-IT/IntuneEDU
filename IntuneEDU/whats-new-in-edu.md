---
# required metadata

title: What's new
titleSuffix: Intune for Education
description: Find out what's recently released in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 12/3/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 7d8dfd82-8cee-4874-85f6-edaf84e49c4c
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience: 
.#ms.devlang:
#ms.reviewer: rashok
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---
# What's new in Intune for Education
Learn what’s new in Intune for Education. Find out about upcoming changes, product notices, and features from previous releases.

## November 2018 

### Remote Autopilot Reset 
You can now invoke Autopilot Reset remotely using the Intune for Education console. Autopilot Reset removes all user data including user-installed apps and personal settings and keeps the device enrolled in Intune so the device is kept up to date with all the latest apps, policies, and settings. With this feature, you can quickly wipe and reconfigure students' PCs in bulk to prepare them for a new school year.

### New features for iOS management
- Intune for Education now displays location information for your Apple School Manager VPP tokens, so you can easily identify your VPP tokens from both Intune for Education and Apple School Manager. 
- You can give your VPP tokens nicknames in Intune for Education for easy labeling and organization. 
- Enrollment is now even faster for your iOS devices when you set up an MDM Server Token. Intune for Education automatically configures enrollment settings, so the devices associated with the MDM Server Token have fewer Setup Assistant screens to tap through. 
 
### Delete Device
You can now delete a device in the Intune for Education console. Deleting a device:
- unenrolls the device in Intune.
- removes the device record from Azure Active Directory so the device is no longer part of your environment.
 
### Immersive Reader for all Tenants 
Your Windows Store for Education inventory gets unlimited licenses for Immersive reader when you sign up for Intune for Education. Immersive Reader is a learning tool that creates a reading experience with accessibility and comprehensions for learners of all ages and abilities. Learn more about Immersive Reader here.
 
### Effective Policy Page
The effective policy page shows all apps and settings applied to a user/device combination based on group memberships. From this page you can see settings that might be in conflict and troubleshoot the issues. You can reach the effective policy page in two ways:
- click on a user and then click on a device that user has recently checked in with.
- click on a device and then click on a user that has recently checked in on that device.



## July 2018 

### All new support for iOS classroom devices  

Intune for Education now supports iOS device management in the classroom. We've added new features and pages to Intune for Education to make the setup and management process easy for everyone involved. From the dashboard, you'll have everything you need to successfully setup, configure, and enroll devices.  

* Setup iOS device management: We've added a new page with [step-by-step guidance](setup-ios-device-management.md) to help you quickly connect your Apple accounts to Intune for Education. On-screen indicators let you clearly see the required and optional steps, the ones you've successfully completed, and the ones that are nearing expiration.
* Express configuration: Just like our Windows 10 experience, but tailored to iOS devices, [express configuration for iOS](express-configuration-intune-edu.md) helps you quickly assign and change apps and settings. Simply choose a group of users or devices and select from our Microsoft-recommended settings. These [recommendations are preselected](edu-express-config-settings-ios.md), but you can change them at any time to match your school's own policies.  
* Apps and settings: We've added separate app and device setting views to help you focus on either [iOS](all-edu-settings-ios.md) or [Windows 10](all-edu-settings-windows.md) device management. With added [Apple VPP support](add-vpp-apps-ios.md), you can sync your VPP-purchased apps with Intune for Education and assign them directly from the dashboard. 
* Dynamic grouping: Now you can apply a specific device platform rule to your [dynamic groups](create-groups.md#dynamic-groups). Create a rule to apply to devices or students on Windows 10 *or* iOS devices.  

Get more details and learn how to navigate new pages and workflows in the [Intune for Education](what-is-intune-for-education.md) documentation.   

## January 2018

### History of group actions taken by admins

You can now view a history of all actions taken by admins to change group admins, apps, and settings for their approved groups. You can find the log of this history in **Groups** > **History**.

### Windows Defender report

We've added a new report. On the Reports page, you can select **Windows Defender report** from the list of reports. This lets you view Windows Defender device health status for all your devices. You can see what this looks like in the [What are reports?](what-are-reports.md) doc.

### Use role-based access control to enable group admins

You can now choose groups of people to manage settings for other groups. For example, you could have a group called *High School Admins*, where the members are your team of admins for high schools in your district. The *High School Admins* group could be given permission to manage settings for groups of high school students. Find out more in the [What are groups? doc](what-are-groups.md).

### User and device search

We've added two new options to the sidebar: **Users** and **Devices**. You can use these to search for individual users or devices, and quickly open the **Details** for these items. You can add these searches to the sidebar by **See all** > **Star button (Favorite)** to add them to your favorites list.

### Remote actions

You can now take remote actions on your users and devices. Select the device you want to take action on, then choose one of the following actions from the details page:

#### Devices

- Restart
- Reset to factory settings
- Sync
- Remove from management

#### Users

- Reset password

Find out more about [remote actions](edu-device-remote-actions.md).

### Wi-Fi profiles

We've added a new option to the sidebar for **Wi-Fi profiles**. This lets you define Wi-Fi settings that you can assign to different devices, users, and groups.

## October 2017

### Dynamic groups

Define rules and we'll create groups that automatically populate based on them.

### New app status

When adding an app, you'll now see a per-device and per-user status of app installs.

### Updated details pages

Select a user or device in one of your groups. A pane will now slide up from the bottom of the screen that lets you get more information on that object, and the status of the apps and settings that you've assigned to it.

## May 2017 (initial release)

### Intune for Education is now available!

We have launched the Intune for Education portal. Intune for Education is a streamlined experience for schools and educational organizations to manage Windows 10 devices. Find out more about Intune for Education in these docs.

## Next steps

- [Find out more about Intune for Education](what-is-intune-for-education.md)
- [Find out more about the full device management experience with Intune](https://docs.microsoft.com/intune/understand-explore/introduction-to-microsoft-intune)
