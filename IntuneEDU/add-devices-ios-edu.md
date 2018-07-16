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
* Enable Intune for iOS device management by [setting up the Apple Push MDM certificate and Apple MDM Server tokens](setup-ios-device-management.md#add-an-mdm-push-certificate).
* [Sync your Apple MDM Server tokens](setup-ios-device-management.md#sync-managed-devices) with Intune for Education and see a list of ready-to-enroll devices.  

> [!NOTE]
> Make sure your devices are connected to the Internet and your account has enough Intune for Education device licenses to complete setup. Find out more about licensing in [Assign licenses to users](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune-step-4).

## Pre-configured enrollment profile
Intune for Education creates and assigns each synced device a school-optimized enrollment profile.  

Enrollment profiles are configured to tell the device how to set itself up and enroll in management. Intune configures the settings to help speed up your enrollment.  When you power on the device, the enrollment profile immediately begins setting up your device.

## List of preconfigured settings
During initial device setup, devices enroll with the following configurations:

* No user affinity
* Supervised mode enabled
* Blocked from syncing or pairing with other devices
* Locked enrollment, meaning users can't change management settings on their devices


The following Setup Assistant settings are hidden during enrollment:
* Passcode setup
* Location Services
* Device restore
* iCloud & Apple ID
* Touch ID setup
* Apple Pay setup
* Display Zoom options
* Siri setup
* Diagnostics Data options

The following Setup Assistant setting is shown during enrollment:
* Terms and Conditions

### What is Setup Assistant?
The first time that you turn on your device, Intune for Education launches the iOS out-of-the-box experience, called *Setup Assistant*. Setup Assistant walks you through a series of screens and prepares your device for school use.  

## Enroll a device

These steps can be done by a delegated admin or [enrollment manager](add-enrollment-managers.md), such as a teacher or IT person, or by your students. If students and teachers are part of the initial device setup, consider pointing them to this article.

1. Turn on your iOS device. 
2. After you select your **Language**, connect your device to Wi-Fi.
3. On the **Set up iOS device** screen, select **Set up as new device**.
4. After you're connected to Wi-Fi, the **Configuration** screen appears, with:  

**[Your School] will automatically configure your device. Configuration allows [Your School] to manage this device over the air.**   

**An administrator can help you set up email and network accounts, install and configure apps, and manage settings remotely. An administrator may disable features, install and remove apps, monitor and restrict your Internet traffic, and remotely erase this device.**  
      
**Configuration is provided by:
   [Your School's] iOS Team
   [Address]**

5. Agree to the **Terms and Conditions**. Then decide if you want to send diagnostic information to Apple.  

## Next steps
- [Find out more about the **Set up School PCs** app](https://docs.microsoft.com/education/windows/use-set-up-school-pcs-app)
- [Find out more about the full experience adding devices into Intune](https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune)
