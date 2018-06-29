---
# required metadata

title: iOS device enrollment profile settings
titleSuffix: Intune for Education
description: Describes the default settings applied to iOS devices during initial startup
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/26/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 2221009e-68cf-4171-8118-0d750b0f35f1
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
# iOS device enrollment profile settings

After you sync your devices from Apple School Manager, Intune for Education creates and assigns each device a school-optimized enrollment profile. The enrollment profile is pre-configured to tell the device how to set itself up and enroll in management. Nearly no work is required from you to enroll your device. 

## What is Setup Assistant?
The first time that you turn on your device, Intune for Education initiates the iOS out-of-the-box experience, called Setup Assistant. Setup Assistant walks you through a series of screens and prepares your device for school use.   

## List of preconfigured settings
During initial device setup, devices enroll with the following configurations:

* No user affinity
* Supervised mode enabled
* Blocked from syncing or pairing with other devices
* Locked enrollment, meaning users cannot change management settings on their devices


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





