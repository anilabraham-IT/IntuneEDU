---
# required metadata

title: Enroll iOS devices in management
titleSuffix: Intune for Education
description: Learn how to set up Windows 10 devices for Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 05/16/2019
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

## Preconfigured enrollment profile  
Intune for Education creates and assigns each synced device a school-optimized enrollment profile.  

Enrollment profiles are configured to tell the device how to set itself up and enroll in management. Intune configures the settings to help speed up your enrollment.  When you power on the device, the enrollment profile immediately begins setting up your device.

## Preconfigured settings  
During initial device setup, devices enroll with the following configurations:

* No user affinity
* Supervised mode enabled
* Blocked from syncing or pairing with other devices
* Locked enrollment, meaning users can't change management settings on their devices  

Intune for Education applies a naming scheme to devices that you enroll with an MDM server token. By default, devices are named with their device serial number. You'll have the option to add on a custom device name when you set up your MDM server token.  

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

Walk through the following steps to complete device enrollment.

1. Turn on your iOS device. 
2. After you select your **Language**, connect your device to Wi-Fi.
3. On the **Set up iOS device** screen, select your **Country/Region**.
4. Follow the instructions on screen to automatically or manually connect to Wi-Fi. After you're connected, the **Configuration** screen appears, with enrollment details.  
5. Agree to the **Terms and Conditions**. Then decide if you want to send diagnostic information to Apple.  

## Next steps
Now that devices are setup and ready for school use, learn how to update, monitor, and troubleshoot them.   
* Add more [free](add-apps-ios.md) and [VPP](add-vpp-apps-ios.md) iOS apps throughout the school year
* Assign [group admins](group-admin-delegate.md) to help you manage classroom settings within your school or across the district
* Learn how [settings inheritance](settings-inheritance.md) affects new groups
* Review [reports](what-are-reports.md) to pinpoint and troubleshoot errors 
* Renew [iOS certificates and tokens](renew-ios-certificate-token.md) every year
