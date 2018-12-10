---
# required metadata

title: Use Autopilot Reset to reconfigure devices with Intune for Education
titleSuffix: Intune for Education
description: Learn how to Autopilot Reset in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 12/3/2018
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
#ms.reviewer: rashok
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Autopilot Reset
You can use Autopilot Reset to remove personal files, apps, and settings from your devices. The devices remain enrolled in Intune and are returned to a fully-configured or known IT-approved state.
You can Autopilot Reset a device locally or remotely from the Intune for Education portal.
Using the Intune for Education portal, you avoid the need for IT staff to visit each device to start the process. From the portal, you can reset a single device or do a bulk reset for all devices in a group. Resetting all devices in a group lets you quickly wipe and reconfigure student devices to prepare them for the new school year.
After a reset, the original settings are applied to the device and then it syncs with Intune to get the latest policies.
## Requirements
Using Autopilot Reset locally is only available for devices running Windows 10 version 1709 or later.
Using Autopilot Reset remotely is only available for devices running Windows 10 build 17672 or later.

## Use Autopilot Reset locally
If you need to wipe a single device, you can do so directly on the device.
On the device, press CTRL+WIN+R.
## Use Autopilot Reset remotely for a single device
1.	In Intune for Education, choose **Groups** > choose a group > choose a device > **Autopilot Reset**  > **Autopilot Reset**.
2.	A notification shows when the reset was initiated. The device will be reset the next time it connects to the Internet.
## Use Autopilot Reset remotely for devices in bulk
1.	In Intune for Education, choose **Groups** > choose the group > **Autopilot Reset all devices**.
2.	In the **Autopilot Reset group** box, type the name of the group in the text box and then choose **Autopilot Reset**.
3.	A status list appears If any of the devices don’t support remote Autopilot Reset. Each device will be reset the next time that it connects to the Internet.

## Next steps
[Manage devices with remote actions](edu-device-remote-actions.md)



