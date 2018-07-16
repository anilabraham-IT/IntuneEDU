---
# required metadata

title: Add a Wi-Fi profile for Windows and iOS devices
titleSuffix: Intune for Education
description: Learn how to create a Wi-Fi profiles for your devices in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
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

A Wi-Fi profile describes how to connect to your school's network. When you assign the profile to a user or device group, the group can automatically access your school's network from their devices. Profiles eliminate the need for students and teachers to manually connect to the network.

This article describes how to configure profiles for Windows 10 and iOS devices.

## Supported device platforms
Wi-Fi profiles are supported on Windows 10 devices, and on iOS devices bought through Apple DEP. 

## Configure your profile
Windows 10 and iOS Wi-Fi configurations vary slightly. Because of the differences, you must create an individual Wi-Fi profile for your school's Windows 10 devices, and an individual one for your school's iOS devices.
1. Sign in to Intune for Education > **Wi-Fi profiles**.
2. Select the device platform you're configuring a profile for.  
    a. To create a profile for a Windows device, click **Add Windows 10 Wi-Fi profile**.   
    b. To create a profile for an iOS device, click **Add iOS Wi-Fi profile**. 
3. Enter the details of your school's wireless network. Use the tables below to help you as you fill out these settings. Settings differ between device platforms so make sure you look at the table appropriate for your device.
4. When you're done, click **Save**.

### Wi-Fi settings for Windows 10 devices
|Setting |Description  |
|---------|---------|
|Profile name    |  Enter a unique name for your profile.| 
|Network name (SSID)    |  Enter a display name for your wireless connection. People will see this name when they browse the list of available networks from their device.  |
|Security type   |  Select the security protocol to use to authenticate to the Wi-Fi network. Intune for Education supports WPA2-Personal and Open. Select Open if you require no password to access your school's network. This type of network is unsecured, meaning anyone can access it.| 
|Password    |  Enter the password for your Wi-Fi network. Password must be 8-63 characters long. | 
|Confirm password| Reenter the password for your Wi-Fi network.|
|Description| Briefly describe who the network is for or how it will be used.|  

### Wi-Fi settings for iOS devices
|Setting |Description  |
|---------|---------|
|Profile name    |  Enter a unique name for your profile.       | 
|Network name (SSID)    |  Enter a display name for your wireless connection. People will see this name when they browse the list of available networks from their device.        |
|Security type   |  Select the security protocol to use to authenticate to the Wi-Fi network. Intune for Education supports WPA2-Personal and Open. Select Open if you require no password to access your school's network. This type of network is unsecured, meaning anyone can access it.       |  
|Password    |  Enter the password for your Wi-Fi network. Password must be 8-63 characters long. | 
|Confirm password| Reenter the password for your Wi-Fi network.|
|Connect automatically   |  If enabled, assigned devices within range of the network will automatically connect. If not enabled, your students or teachers must manually select the network from the list of available networks.       | 
|Make a hidden network   | If enabled, your network won't appear to users in the list of available networks. They'll have to manually type in the network name (SSID) to connect to it.       | 
|Configure proxy settings| When enabled, you can configure proxy settings for your school's network.|
|Proxy settings   |  Select if you want to manually configure your proxy settings or if you want to enable a proxy script to automatically detect settings.     | 
|Proxy server address   | Type in the IP address of the proxy server. Not applicable if you selected to automatically detect proxy settings.      |
|Proxy server port| Type in the virtual port number where the proxy is located.    | 
|Proxy server URL  | Type in the server URL you want to use to automatically connect to the proxy server. Not applicable if you selected to manually configure proxy settings.       |   

## Assign profile to groups
1. Go to the portal's left-navigation bar and click **Groups**.
2. On the group's page, click the **Settings** tab.
3. Click to expand the appropriate group of device settings for your OS.
4. Click Wi-Fi profiles and select a profile to assign in to the group. Deselect a profile to remove its assignment to the group.
5. Click **Save**.

## Next steps
- [Find out more about the full groups management experience in Intune](https://docs.microsoft.com/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)
