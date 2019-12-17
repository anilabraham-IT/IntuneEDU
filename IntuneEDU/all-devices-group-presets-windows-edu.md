---
# required metadata

title: Windows 10 All Devices group presets
titleSuffix: Intune for Education
description: See a list of the Windows 10 device settings that are preset at time of signup
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 12/17/2019
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
#ms.reviewer: elcox
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# All Devices group presets for Windows 10
After you sign up for an account, Intune for Education presets some of the settings in the All Devices group. These settings help you get a head start at managing Windows 10 devices in the classroom. To adjust the settings, go to Intune for Education > **Groups** > **All Devices** > **Windows device settings**.  

> [!NOTE]
> These presets are applied automatically for new tenants. If your school is already set up in Intune and then you sign up for Intune for Education, these presets won't be applied automatically. This behavior is intentional and prevents unwanted changes to your existing environment. You can, however, see the recommended presets and decide if you want to apply them yourself.       

For a list and descriptions of all Windows 10 device settings, see [Windows 10 device settings](all-edu-settings-windows.md).  

|Category|Setting|Preset value|
|---|---|---|
|Apps|Require Microsoft Store for Education apps to be installed from the private store|Require|
|Apps|Trusted apps|Block|  
|Apps|Untrusted apps|Block| 
|Enrollment controls|Block manual unenrollment|Block|
|Enrollment controls|Block Autopilot Reset|Disable|
|Enrollment controls|Block adding provisioning packages|Block|
|Enrollment controls|Block removing provisioning packages|Block|
|Microsoft Edge|Block untrusted browser extensions |Block|
|Microsoft Edge|Block overriding security warnings |Block|
|Microsoft Edge|Use cookies|User-defined
|Network and connectivity|Block Bluetooth Swift Pair notifications |Block
|Security|Block user access to Windows Defender settings|Enable
|Security|Enable real-time monitoring|Enable
|Security|Enable behavior monitoring|Enable
|Security|Prompt users to submit suspicious files to Microsoft|Never send data
|Security|Type of system scan to perform|Quick scan|
|Security|Daily quick scan time|2 AM|
|Security|Scan all downloaded files|Enable|
|Security|Scan scripts run in Microsoft web browsers|Enable|
|Security|Scan removable drives during full scan|Enable|
|Security|Scan files opened over the network|Enable|
|Security|Scan remote folders during full scan|Enable|
|Security|Scan archive files|Enable|
|Security|Scan incoming email|Enable|
|Security|Scan for malware when files or programs are opened|Monitor all files|
|Security|Days before quarantined malware is removed|0|
|Security|Set anti-malware update frequency|8 hours|
|Security|Enable cloud-delivered protection|Enable|
|Security|Enable Network Inspection Service|Enable|
|Updates and upgrade |Branch readiness level|Semi-Annual Channel|
|Updates and upgrade |Configure how and when updates are installed|Automatically install and reboot without end-user control| 
|Updates and upgrade |Days to defer feature updates after they become available |0|
|Updates and upgrade |Days to defer quality updates after they become available  |0|
|Updates and upgrade |Delivery Optimization mode|HTTP with peering NAT |
|Updates and upgrade |Switch out of S Mode|Keep in S Mode|
|User experience|Block Cortana|Block|
|User experience|Send diagnostic data|Basic|
|User experience|Block Windows Spotlight|Block|  

By default, Intune for Education is set up to automatically enroll Windows 10 devices. Automatic enrollment connects Azure Active Directory and Intune so that when a user signs in with their school account, their device will automatically enroll with Intune. To learn more about Windows 10 automatic enrollment, see [Enable Windows 10 automatic enrollment](https://docs.microsoft.com/intune/enrollment/windows-enroll#enable-windows-10-automatic-enrollment). 
 
By default, Intune for Education blocks users from enrolling their personal Windows devices. This default ensures that personal devices aren't accidentally enrolled.  

## Next steps
For the full list of Windows 10 settings available in Intune for Education, see [All Windows 10 settings](all-edu-settings-windows.md).  

Custom settings are available in Intune in the Azure portal. For more information, see [Use custom settings for Windows 10 devices](https://docs.microsoft.com/intune/custom-settings-windows-10).  
