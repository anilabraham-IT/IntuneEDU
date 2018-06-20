---
# required metadata

title: What are tenants?
titleSuffix: Intune for Education
description: Learn how to manage your tenant with tenant-wide settings.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 01/17/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 50bd115f-a167-456a-910d-8f31ec17a422
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

# Overview of tenant settings

*Tenant* refers to your organization's instance of Intune for Education. When you modify settings at the tenant level, changes do not impact groups, such as **All Students**. Rather, they affect every device that is managed in your organization and each of the devices' users.  (//lenewsad: how does it affect them?) Modifications are made to your entire subscription and to all of your licenses. //lenewsad: what does this last sentence mean? What settings can i change in tenant settings that are relavant to the entire EDU subscription and all licenses?

Intune for Educations has both **General** settings and **iOS Device Management** tenant settings. 

The **General** page of tenant settings asks for contact information about your organization and its IT resources. Most of this information is optional but is useful to provide an IT point of contact for students and faculty.

THe **iOS Device Management** page asks for information about your Apple accounts, and is a requirement for organizations who wish to manage their iOS devices under Intune.

Only Intune for Education admins (//lenewsad: What do we mean here by "admins?" Is that the name of the role they need to be assigned in big intune?) can see and change tenant settings.

## Edit general tenant settings
To edit tenant settings:
1. Sign in to the Intune for Education portal. 
2. Go to the left-side navigation bar and click **Tenant Settings** > **Edit**.![Screenshot of the "Tenant Settings" option in Intune for Education console showing school, support website, and other information. ](./media/tenant-001-settings-screen.png)
3. Enter the details of your organization. Some of this information will be visible to students and faculty as they use their devices. If your organization has a specific IT department or person that troubleshoots devices, provide their contact information here.

|Setting |Description  |Example  |
|---------|---------|---------|
|Organization name     |  Your organization's name appears in text throughout the Company Portal.       |         |
|IT department contact name    | Name of the contact person that provides IT-related support.        |         |
|IT department phone number   | Phone number that is made visible to students and faculty in the Company Portal so that they can contact you for support.        |         |
|IT department email address     | Email address that is made visible to students and facutly in the COmpany POrtal so that they can contact your for support.        |         |
|Privacy statement URL    |  Appears as a link in the Company Portal. Sends students to your organization's privacy statement.       |         |
|Additional information     | Additional details such as office hours, address, or alternative phone number.        |         |
|Support website URL    | Appears as a link the Company Portal. Sends students and faculty to your organization's support website.        |         |
|Website name    | Display name for your organization's support website.        |         |

## Force a sync
//lenewsad: I don't see this functionality in the test environment. Has this since been removed?

Tenant settings are also where you can force a sync between Intune for Education and Microsoft Store for Education if app purchases are taking too long to appear in Intune for Education.

## Find out more

- [Find out more about setting up role-based access in the full management experience in Intune](https://docs.microsoft.com/intune-azure/access-control/role-based-access-control)
