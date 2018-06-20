---
# required metadata

title: Add a Wi-Fi profile for Windows and iOS devices
titleSuffix: Intune for Education
description: Learn how to create a Wi-Fi profiles for your devices in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/19/2018
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

Wi-Fi profiles contain the network settings that are necessary to connect to a network. When a profile is assigned to a user or device group, the group is able to access your school's network without further configurations. 

This article describes how to configure a profile for Windows 10 and iOS devices.

## Supported device platforms
Wi-Fi profiles are supported on Windows 10 devices and iOS devices purchased through Apple DEP.   

## Configure your profile
1. Sign in to Intune for Education > **Wi-Fi profiles**.
2. Select the device platform you are configuring a profile for.
    a. If you are creating a profile for a Windows device, click **Add Windows 10 Wi-Fi profile**. 
    b. If you are creating a profile for an iOS device, click **Add iOS Wi-Fi profile**. 
3. Enter the details of your school's wireless network. The table below lists each setting, a description, and the device platform it is applicable to. Settings vary between Windows 10 and iOS devices.
4. When you are done, click **Save**.


|Setting |Description  |Applicable to what devices|
|---------|---------|---------|
|Profile name    |  Enter a unique name for your profile.       |  Windows 10, iOS       |
|Network name (SSID)    |  Enter a display name for your wireless connection. People will see this name when they browse the list of available networks from their device.        |Windows 10, iOS        |
|Security type   |  Select the security protocol to use to authenticate to the Wi-Fi network. Intune for Education supports WPA2-Personal and Open. Select Open if you require no password to access your school's network. This type of network is unsecured, meaning anyone can access it.       |  Windows 10, iOS       |
|Password    |  Enter the password for your Wi-Fi network.       |  Windows 10, iOS       |
|Connect automatically   |  If enabled, when a device is within range of the network, it will automatically connect. If not enabled, your students or teachers must manually select the network from the list of available networks.       | Windows 10, iOS        |
|Make a hidden network   | If enabled, your network will not be appear to users in the list of available networks.        | Windows 10, iOS        |
|Proxy settings   |  Select if you want to manually configure your proxy settings or if you want to enable a proxy script to automatically detect settings.     |  iOS only      |
|Proxy server address   | Type in the IP address of the proxy.       |  iOS only       |
|Proxy server URL  | Type in the server URL for the proxy server.        |  iOS only       |
|Port number  | Type in the computer port number where the proxy is located.    |  iOS only       |

//lenewsad Could not verify the settings name for address and URL. Are they correct?


## Assign profile to groups
2. Click the **Groups** tab.
3. On the left side of the Wi-Fi page, click the profile you want to assign.
4. The table lists the groups that the profile is currently assigned to. To edit or add to the group assignment, click the group > **Go to group page**.
5. On the group's page, click the **Settings** tab.
6. Click to expand the appropriate group of device settings for your OS.
7. Click Wi-FI profiles and select a profile to assign in to the group. Deselect a profile to remove its assignment to the group.
8. Click **Save**.

## Find out more
- [Find out more about the full groups management experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
