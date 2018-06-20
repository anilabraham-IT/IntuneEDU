---
# required metadata

title: Set up Intune for Education on iOS
titleSuffix: Intune for Education
description: Learn how to set up Intune for Education in your organization.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 05/10/2017
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 9d0466c5-d69d-4b85-814a-76e63dd65e63
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

# Set up Intune for IOS devices

Complete the following steps to prepare your classrooms for Intune for Education.

1. Sign in to the Intune for Education portal with your school credentials.
2. [Set up school data](what-is-school-data-sync.md) — Import or sync your school information with Microsoft's School Data Sync (SDS). School Data Sync is not required to configure your student and teacher information. 
3. Alternatively, or in addition to Microsoft SDS, manually create [groups](what-are-groups.md) in Azure Active Directory. 
4. [Add iOS devices to Intune management](how-do-i-add-devices.md) — Upload an Apple MDM Push Certificate to Intune for Education and set up a Device Enrollment Program (DEP) token.
5. Install purchased iOS apps on devices. Configure your Apple Volume Purchase Program account. When connected, Intune can install your purchased apps to your Intune-managed devices.
6. [Launch Express Configuration](what-is-express-configuration.md) — Assign apps and settings to the groups of students and teachers in your organization. 
7. Distribute apps and settings to your Windows and iOS devices. 

## Find out more about what's inside the Azure portal
- [Tenant-level tasks in Intune for Education](what-are-tenants.md)
- [Full management experience in Intune](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune)
- [Manage groups in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-groups-create-azure-portal)
