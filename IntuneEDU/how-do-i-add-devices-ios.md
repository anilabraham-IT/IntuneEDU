---
# required metadata

title: Enroll iOS devices in management
titleSuffix: Intune for Education
description: Learn how to set up Windows 10 devices for Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/20/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: c884df47-61a9-4799-a407-8cd311d376d1
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

# Enroll iOS devices in Intune for Education

Devices are ready to power on and enroll in management after you:

* Set up Intune for Education [with school information](what-is-school-data-sync.md) — such as student records, apps, and settings for devices.
* Enable Intune for iOS device management by [setting up the Apple Push MDM certificate and Apple DEP tokens](setup-ios-device-management.md#add-an-mdm-push-certificate).
* [Sync your Apple DEP tokens](setup-ios-device-management.md#sync-managed-devices) with Intune for Education and see a list of ready-to-enroll devices.  

> [!NOTE]
> Make sure your devices are connected to the Internet and your account has enough Intune for Education device licenses to complete setup. Find out more about licensing in [Assign licenses to users](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune-step-4).

## Enroll your devices
iOS devices are enrolled with a pre-configured enrollment profile. Aside from the basic configurations Setup Assistant, no other steps are necessary. 

These steps can be done by a delegated admin or [enrollment manager](add-enrollment-managers.md), such as a teacher or IT person, or by your students. If students and teachers are part of the initial device setup, consider pointing them to this article.

1. Turn on your iOS device. 
2. After you select your **Language**, connect your device to Wi-Fi.
3. On the **Set up iOS device** screen, select **Set up as new device**.
4. After you're connected to Wi-Fi, the **Configuration** screen appears, with:  

**[Your School] will automatically configure your device. Configuration allows [Your School] to manage this device over the air.**   

**An administrator can help you set up email and network accounts, install and configure apps, and manage settings remotely. An administrator may disable features, install and remove apps, monitor and restrict your Internet traffic and remotely erase this device.**  
      
**Configuration is provided by:
   [Your School's] iOS Team
   [Address]**

5. Agree to the **Terms and Conditions**. Then decide if you want to send diagnostic information to Apple.
6. After you complete enrollment, you may receive a prompt to take more actions. Some of these steps might be entering your password for email access or setting up a passcode.

## Next steps
- [Find out more about the **Set up School PCs** app](https://docs.microsoft.com/education/windows/use-set-up-school-pcs-app)
- [Find out more about the full experience adding devices into Intune](https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune)
