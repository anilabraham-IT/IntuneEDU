---
# required metadata

title: Add devices
titleSuffix: Intune for Education
description: Learn how to set up Windows 10 devices for Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 10/24/2018
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

# Add Windows devices

After you've set up Intune for Education with your information — such as student records, apps, and settings for devices — connect the devices to Intune for Education. For new Windows 10 devices, a connection is established during initial device setup.

## Setting up devices with Windows Autopilot
Windows Autopilot is compatible with Intune for Education. However, it is not a feature that's built-in to Intune for Education. To [set up your devices using Autopilot](https://docs.microsoft.com/intune/enrollment-autopilot), you must go to [Intune in the Azure portal](https://portal.azure.com) > Device enrollment > Windows enrollment > Devices.  

## Before you begin
During setup, devices must have:
* Access to the Internet.
* Intune for Education device license. Find out more about the devices license in the Intune [licenses docs](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune-step-4).  

## Windows device setup
Complete the following steps to add your Windows 10 devices to Intune for Education.

1. Power on the new Windows 10 device. Follow the standard Windows device setup. 
2. On the **Who owns this PC?** screen, select **My work or school owns it**.

   ![Screenshot of the "Who owns this PC?" screen in Windows setup](./media/devices-001-who-owns-this-pc.png)

2. On the **Choose how you'll connect** screen, select **Join Azure AD**.

   ![Screenshot of the "Choose how you connect" screen in Windows setup](./media/devices-002-how-you-connect-pc.png)

3. Enter the account details for the Intune for Education admin or enrollment manager. Then click **Next**.

4. Your device [authenticates with Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access) and identifies with the group or groups it belongs to.  
After setup is complete, the device will receive all apps and settings that you assigned to its group.

## Set up School PCs app
Add Windows devices to Intune through the Set up School PCs app. The app walks you through how to configure and save a single device profile that you can distribute to multiple PCs. A USB drive is used to save and download the profile to each device during device setup. 

For more information about the app, see [**Set up School PCs** app](https://docs.microsoft.com/education/windows/use-set-up-school-pcs-app).

[Want to find about more about the full experience adding devices into Intune?](https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune)
