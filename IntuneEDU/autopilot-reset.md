---
# required metadata

title: Use Autopilot Reset to reconfigure devices with Intune for Education
titleSuffix: Intune for Education
description: Learn how to Autopilot Reset in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 12/13/2019
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: madakeva
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Autopilot Reset
You can use Autopilot Reset to remove personal files, apps, and settings from your devices. The devices remain enrolled in Intune and are returned to a fully-configured or known IT-approved state.
You can Autopilot Reset a device locally or remotely from the Intune for Education portal.  

Using the Intune for Education portal, you avoid the need for IT staff to visit each device to start the process. From the portal, you an wipe a device and then reconfigure it to prepare it for a new student or classroom.  

After a reset, the original settings are applied to the device and then it syncs with Intune to get the latest policies. When Autopilot reset is used on a device, the device's primary user will be removed. The next user who signs in after the reset will be set as the primary user.   

## Requirements
Using Autopilot Reset locally is only available for devices running Windows 10 version 1709 or later.
Using Autopilot Reset remotely is only available for devices running Windows 10 build 17672 or later.

## Use Autopilot Reset locally
If you need to wipe a single device, you can do so directly on the device. On the device, press CTRL+WIN+R. After pressing Ctrl+WIN+R, you’ll have to authenticate with admin credentials in order to trigger the reset.

## Use Autopilot Reset remotely for a single device
1. In Intune for Education, choose **Groups** > choose a device group.
2. Select a device > **Autopilot Reset**. To confirm the reset, select **Autopilot Reset** again.
2.	A message appears when the reset is initiated. The device will reset the next time it connects to the Internet.  

## Next steps
[Manage devices with remote actions](edu-device-remote-actions.md)



