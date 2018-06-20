---
# required metadata

title: Add a Wi-Fi profile
titleSuffix: Intune for Education
description: 
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 02/13/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 4b570196-a640-4d13-8e01-8e8553ce1468
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

# Add a Wi-Fi Profile

Wi-Fi profiles contain the network settings that are neccessary to connect to a network. When a profile is assigned to a user or device group, the group is able to access your school's network without further configurations. This article describes how to configure a profile for your iOS and Windows devices.

## Supported device platforms
Wi-Fi profiles are supported on the following device platforms:
* Which
* Ones
Can they export a previous configuration from another device?

## Configure your profile
1. From the Intune for Education dashboard, go to Wi-Fi profiles.
2. If you are creating a profile for a Windows device, click Add Windows 10 Wi-Fi profile. If you are creating a profile for an iOS device, click Add iOS Wi-Fi profile. 
3. Enter the details of your school's wireless network.
    * Profile name: Enter a unique name for your profile.
    * Network name (SSID): Enter a display name for your wirless connection. This is the name people will see when they browse the list of available networks from their device.
    * Security type: Select the security protocol to use to authenticate to the Wi-Fi network. Intune for Education supports WPA2-Personal and Open.
        * WPA2-Personal: IX Note: WHat does this mean?
        * Open (no authentication): Select if you require no password to access your school's network. This type of network is unsecured, meaning anyone can access it.
    * Password: Enter the password for you Wi-Fi network. 
    * Connect automatically: (IX note: what is default setting?) If enabled, when a device is within range of the network, it will automatically connect. If not enabled, your students or teachers must manually select the network from the list of available networks.
    * Make this a hidden network: If enabled, your network will not be appear to users in the list of available networks.
    * Configure proxy settings:  What is this 
        * Proxy settings: Difference between Manual and Automatic?
        * Proxy server address:
        * Proxy server URL: And this
        * Port number: Ya this too
4. Click **Save**.

## Assign profile to groups
2. Click the **Groups** tab.
3. On the left side of the Wi-Fi page, click the profile your want to assign.
4. The table lists the groups that the profile is currently assigned to. To edit or add to the group assignment, click the group > **Go to group page**.
5. On the group's page click the Settings tab.
6. Click to expand the appropriate group of device settings for your OS.
7. Click Wi-FI profiles and select a profile to assign in to the group. Deselect a profile to remove its assignment to the group.
8. Click **Save**.

## Find out more
- [Find out more about the full groups management experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
