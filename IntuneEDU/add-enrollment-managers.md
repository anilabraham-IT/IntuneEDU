---
# required metadata

title: Add enrollment manager
titleSuffix: Intune for Education
description: Learn the role of Enrollment Managers in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 01/17/2018
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

# Add Enrollment Managers

Grant device enrollment permissions to your existing users. Users with device enrollment manager accounts can  enroll up to 1000 Windows 10 devices, and download school apps. (Is the latter correct?) Enrollment manager accounts are helpful in large organizations that have thousands of shared student devices to enroll. 

Users must exist in the Azure portal to be added as device enrollment managers.

Device enrollment permissions cannot be used with these other enrollment methods: Apple Configurator with Setup Assistant, Apple Configurator with direct enrollment, Apple School Manager (ASM), or Device Enrollment Program (DEP).  (Which of these can I delete?)

<IX: how does one become qualified to be an enrollment manager? Will everyone in the entire org show up in the list?>

  ![Dashboard left hand side](./media/dashboard-002-left-sidebar-list.png)

1. Go to the Intune for Education portal > Enrollment Managers.
2. **Click Assign enrollment permissions**.
3. Click the user that you want to assign permissions to. If you know the name of the user, search for them in the search box.
4. Click **Save**.
5. To remove permissions from a user, go to the left side of the screen and click their name. 
6. Click **Remove enrollment permissions**.
7. Click **Remove** to confirm your action. Removing a device enrollment manager does not affect enrolled devices.
  ![Remove enrollment permissions button selected while viewing an individual Enrollment Manager's page](./media/enroll-mgrs-003-remove-enrollment-permissions.png)

- [Find out more about the full device enrollment manager experience in Intune](https://docs.microsoft.com/intune/deploy-use/enroll-corporate-owned-devices-with-the-device-enrollment-manager-in-microsoft-intune)
