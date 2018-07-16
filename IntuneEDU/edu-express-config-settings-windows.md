---
# required metadata

title: Express Configuration default device settings for Windows 10
titleSuffix: Intune for Education
description: Describes the default settings for Windows 10 devices in Intune for Education.
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
# Default Windows 10 configurations in Express Configuration
Express Configuration comes preset to help you quickly set up your iOS devices. Intune for Education chooses options that are both Microsoft-recommended and best for school environments. This article lists each of those settings and their default behavior. 

 Make changes to fit your school's rules and policies, or click straight through the settings page to apply the preset recommendations. 

For the complete list of settings and descriptions, see [All iOS settings in Intune for Education](all-edu-settings-windows.md). 


## Basic device settings  
|Setting|Suggested value| 
|---|---|
|Block manual unenrollment|Block users from manually unenrolling devices from management.|
|Block camera|Block user access to the device camera.|
|Block removable storage|Block users from using removable storage such as USB drives and external hard drives.|
|Block Internet sharing|Block users from using Internet Sharing to share the device’s Internet connection.|
|Block Cortana|Block Cortana, the digital assistant built into Windows 10 that can answer questions and perform tasks.|
|Block adding provisioning packages|Block users from adding new provisioning packages containing device settings.|
|Block removing provisioning packages|Block users from removing provisioning packages containing device settings.|
|Block changing date and time settings|Block users from changing the device date and time settings.|
|Block changing language settings|Block users from changing the device language.|
|Block changing device region settings|Block users from changing region settings, such as country and language.|
|Block location services|Block apps from using location services to access the device’s location.|  

## Sign-in settings  

|Setting|Suggested value|  
|---|---|
|Block signing in using Microsoft account|Block users from signing in with their Microsoft account.|  
|Block adding new non-Microsoft accounts|Block users from adding any account other than their Microsoft account. Use this setting if you want to force users to only use their Microsoft accounts for email.||Block signing in using a Microsoft account|   

## Microsoft Edge settings  

|Setting|Suggested value|
|---|---|
|Block InPrivate browsing|Block users from using InPrivate browsing, which stops Edge from saving data like browsing history and cookies.|  
|Block pop-ups|Block websites from opening new windows.|  
|Block password manager|Block users from using the password manager to save passwords.|  
|Block automatically filling form entries|Block saving data entered in a form field online.|  
|Block developer tools|Block users from accessing developer tools.|  
|Block access to about:flags page|Block access to the about:flags page, which contains experimental settings and features.|  



## Microsoft Store settings   
|Setting|Suggested value|  
|---|---|
|Block installing apps from the Microsoft Store for Education|Block users from installing apps from unauthorized locations.|  
|Require Microsoft Store for Education apps to be installed from the private store|Only allow users to install apps from the Microsoft Store for Education that your organization has set up.|  
|Block automatic app updates|Block Microsoft Store for Education apps from being updated automatically.|  
|Shared app data between users|Allow multiple users of shared devices to share app data.|  

## Wireless settings      
|Setting|Suggested value|  
|---|---|
|Block Bluetooth|Block devices from using Bluetooth.|  

## Reset default settings
To restore all apps to their default selections, click **Reset to app selections**. <add screenshot>  
To restore all settings to their default values, click **Reset to suggested defaults**. <add screenshot>  

