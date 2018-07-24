---
# required metadata

title: Windows 10 All Devices group presets
titleSuffix: Intune for Education
description: See a list of the Windows 10 device settings that are preset at time of signup
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
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

# All Devices group presets for Windows 10
After you sign up for an account, Intune for Education pre-sets some of the settings in the All Devices group. These settings will help you get a head start at managing Windows 10 devices in the classroom. To adjust settings, go to the Intune for Education portal > **Groups** > **All Devices** > **Windows device settings**.  

For a list and descriptions of all Windows 10 device settings, see [Windows 10 device settings](all-edu-settings-windows.md).  

|Category|Setting|Preset value|
|---|---|---|
|Windows Defender|Block user access to Windows Defender settings|Enabled
|Windows Defender|Real-time monitoring|Enabled
|Windows Defender|Behavior monitoring|Enabled
|Windows Defender|Prompt users for sample submission|Never send data
|Windows Defender|Type of system scan to perform|Quick scan|
|Windows Defender|Daily quick scan time|2 AM|
|Windows Defender|Scan all downloaded files|Enabled|
|Windows Defender|Scan scripts run in Microsoft web browsers|Enabled|
|Windows Defender|Scan removable drives during full scan|Enabled|
|Windows Defender|Scan files opened over the network|Enabled|
|Windows Defender|Scan remote folders during full scan|Enabled|
|Windows Defender|Scan archive files|Enabled|
|Windows Defender|Scan incoming email|Enabled|
|Windows Defender|Scan file and program activity|Monitor all files|
|Windows Defender|Days before quarantined malware is removed|0|
|Windows Defender|Set update frequency|8 hours|
|Windows Defender|Enable cloud-based protection|Enabled|
|Microsoft Store|Require Microsoft Store for Education apps to be installed from the private store|Require|
|Microsoft Store|Trusted apps|Block|  
|Microsoft Edge|Block developer tools|Block|
|Microsoft Edge|Block Cortana|Block|
|Basic device|Block manual unenrollment|Block|
|Basic device|Block adding provisioning packages|Block|
|Basic device|Block removing provisioning packages|Block|
|Device update|Branch readiness level|Semi-Annual Channel (Targeted)
|Device update|Pre-release features|Not allowed
|Device update|Delivery optimization mode|HTTP blended with peering NAT |
|Device update|Updates and maintenance period|Automatically install and reboot without end-user control|
|Shared device|Optimize devices for shared use|Enabled|  

## Next steps

- [Find out more about the full Windows 10 settings management experience available in Intune](https://docs.microsoft.com/intune/deploy-use/windows-10-policy-settings-in-microsoft-intune)
