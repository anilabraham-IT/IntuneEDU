---
# required metadata

title: Add enrollment managers
titleSuffix: Intune for Education
description: Learn how to add Enrollment Managers in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 08/30/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: b496bc02-714e-4391-b533-4c9bdcf57483
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

# Add enrollment managers  

Give device enrollment permissions to your existing users. Users with device enrollment manager accounts can enroll up to 1000 Windows 10 devices in Intune for Education.

 Enrollment manager accounts are helpful in large organizations that have thousands of shared Windows 10 devices to enroll.  

## Requirements  

Users must exist in the Azure portal to be added as device enrollment managers.

Device enrollment permissions cannot be used with these other enrollment methods: Apple Configurator with Setup Assistant, Apple Configurator with direct enrollment, Apple School Manager (ASM), or Device Enrollment Program (DEP).  

## Assign enrollment permissions  

1. From the Intune for Education dashboard, click **Enrollment Managers**.
2. **Click Assign enrollment permissions**.
3. Choose the user that you want to assign permissions to. If you know the name of the user, you can search for them in the search field.
4. Click **Save**.

## Remove enrollment permissions  
1. From **Enrollment Managers**, go to the left side of the screen and choose a user. 
2. Click **Remove enrollment permissions**.
3. Click **Remove** to confirm your action. Removing a device enrollment manager does not affect enrolled devices.
  ![Remove enrollment permissions button selected while viewing an individual Enrollment Manager's page](./media/enroll-mgrs-003-remove-enrollment-permissions.png)
