---
# required metadata

title: Express Configuration default device settings for Windows 10
titleSuffix: Intune for Education
description: Describes the default settings for Windows 10 devices in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 03/14/2019
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
# Default Windows 10 configurations in Express Configuration
Express Configuration comes preset to help you quickly set up your Windows devices. Intune for Education chooses options that are both Microsoft-recommended and best for school environments. This article lists each of those settings and their default behavior. 

 Make changes to fit your school's rules and policies, or click straight through the settings page to apply the preset recommendations. 

For the complete list of settings and descriptions, see [All Windows 10 settings in Intune for Education](all-edu-settings-windows.md). 


## Accounts and sign-in 

|Setting|What it does|  
|---|---|
|Block adding and signing in with personal Microsoft accounts |Block students and teachers from adding and signing in to personal Microsoft accounts on the device. Personal Microsoft accounts refer to accounts that use a Microsoft domain name, but aren't in your school's Azure Active Directory tenant.|  
|Block adding and signing in with non-Microsoft accounts|Block students and teachers from adding and signing in to non-Microsoft accounts, such as Google, Yahoo, and iCloud. Use this setting to force users to only use their Microsoft accounts for email.|
|Configure preferred Azure Active Directory tenant domain|Configure your school's domain name so that users can sign in to Windows without it. For example, instead of signing in with the username *alain@contoso.com*, a student would only need to sign in with *alain*. This setting prepopulates your tenant domain name, but you can still edit it.|   

## Apps   
|Setting|What it does|  
|---|---|
|Block installing apps from the Microsoft Store for Education|Block users from installing apps from unauthorized locations.|  
|Require Microsoft Store for Education apps to be installed from the private store|Require users to only install apps from the Microsoft Store for Education that your organization has set up.|  

## Enrollment controls  
|Setting|What it does| 
|---|---|
|Block manual unenrollment|Block users from manually unenrolling devices from management.|
|Block adding provisioning packages|Block users from adding new provisioning packages that contain device settings.|
|Block removing provisioning packages|Block users from removing provisioning packages that contain device settings.|  

## Microsoft Edge settings  
|Setting|What it does|
|---|---|
|Configure homepages|Configure how the Microsoft Edge home page appears to students and teachers. **Open custom pages** opens the URL of your choice. The browser will open a new tab for each URL that you add. **Open last session's pages** opens the pages that were active the last time the browser was closed. If you don't configure this setting, users can configure the home page on their own.| 
|Block InPrivate browsing|Block users from using InPrivate browsing, which stops Microsoft Edge from saving data like browsing history and cookies.|  
|Block browser extensions|Block users from installing browser extensions.|
|Block pop-ups|Block websites from opening new windows.|  
|Block password manager|Block users from using the password manager to save passwords.|
|Block automatically filling form entries|Block saving data entered in a form field online.|
|Block Developer Tools|Block users from opening Microsoft Edge Developer Tools. These tools enable users to build and debug webpages.|  

## User experience 
|Setting|What it does| 
|---|---|
|Block camera|Block use of the device camera.|
|Block OneDrive file sync|Block the device from syncing files to OneDrive.|
|Block removable storage|Block the use of removable storage, such as USB drives, SD cards, and external hard drives.|
|Block Cortana|Block Cortana, the digital assistant built into Windows 10 that can answer questions and perform tasks.|
|Block location services|Block apps from using location services to access the device’s location.|  
|Block ending tasks in Task Manager|Block users from using Task Manager to force a program, process, or task to close.|
|Block changing date and time settings|Block users from changing the device date and time settings.|
|Block changing language settings|Block users from changing the device language.|
|Block changing device region settings|Block users from changing region settings, such as country and language.|
|Set custom lock screen image|Add a custom background image to the device sign-in screen. Type in the web link for a .jpg or .png image that's less than 20 MB in size.|
|Set custom desktop image|Add a custom background image to the device desktop. Type in the web link for a .jpg or .png image that's less than 20 MB in size.|
|Block access to the Settings app|Block user access to the entire Settings app.|  

## Reset default settings
To restore all settings to their default values, click **Reset to suggested defaults**.  

