---
# required metadata

title: How should I enroll my devices?
titleSuffix: Intune for Education
description: Get advice for ways to enroll your devices in to Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/18/2019
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 45160df9-126d-4c51-a0d3-0e9fad0fe929
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

# How should I enroll devices?

Learn how to enroll devices under Intune for Education management. To choose the best method for your school, consider the:  
* Size of your district.    
* Type of device recipients.    
* Number of staff available to help.   
 
Read on to determine the best way to enroll devices in your school.  

## When to use Set up School PCs vs Windows Autopilot  
The following table describes when to use the Set up School PCs app and Windows Autopilot for initial device setup. In some cases, you can use both. Use the **Points to consider** column to consider your own school's environment and setup needs.  

|Points to consider| Set up School Pcs |Windows Autopilot  |
|---------|---------|---------|  
|IT staff | Best when unboxing, first power-on, and configuration of devices is performed by the IT Staff.|Best for limiting IT staff intervention; unboxing, first power-on, and configuration of devices can be performed by students and teachers.|
|Device user|  Best for shared devices and for younger students.|Best for single-user devices in user-driven mode and for older students.|
|Apps     | Best for deploying large apps simultaneously on a slower network.|Works well with apps of all sizes.| 
|Network | Reliable internet connection required; best for low bandwidth environments.| Reliable internet connection required; best if students are setting up the devices on their home network (Azure AD only). Consider the network impact of concurrent setup of multiple devices and the amount of data downloaded over the internet.|
|First day of class|Best if students need to use devices immediately.| Best if students need to unbox, connect to network, and wait for devices to configure.|
|Deployment time|Can take as little as a couple of minutes; depends on network speed and app size.|Can take as little as a couple of minutes; depends on network speed and app size.|
|OEMs/Partners|Not applicable.  |Requires registration of device IDs for the Windows Autopilot service by a partner (CSP) or OEM provider. |
|Existing on premises configuration| Supported with Windows Configuration Designer only. | Supports Hybrid AD join.|  

## Run the Set up School PCs app 
Upload a single set of school-optimized settings to each of your Windows 10 PCs. The [Set up School PCs app](https://docs.microsoft.com/education/windows/use-set-up-school-pcs-app) guides you through how to create an installation package that's appropriate for schools. After you're done configuring settings for your network and devices, the app saves the package to a USB drive. Insert the USB drive directly in to each student PC to automatically set up the device for your students. The app is compatible on PCs running Windows 10 version 1803 and earlier.

## Give school faculty enrollment manager permissions
Add enrollment managers, or an enrollment manager account, to allow your staff to help you enroll devices. [Enrollment managers](add-enrollment-managers.md) can enroll up to 1,000 devices.  

## Allow users to enroll their own devices
Allow trusted users to enroll their own devices. These users are able to automatically join their devices to Azure AD.  

## Next steps  

Ready to enroll your devices? Learn how to add [iOS](add-devices-ios-edu.md) and [Windows 10](add-devices-windows.md) devices under Intune for Education management.  

* See the Store documentation to [download the **Set Up School PCs** app](https://www.microsoft.com/store/p/set-up-school-pcs/9nblggh4ls40) from the Microsoft Store. 
* Find out more [about setting up Windows devices in schools](https://docs.microsoft.com/education/windows/set-up-windows-10) from the Microsoft Education > Windows documentation.

