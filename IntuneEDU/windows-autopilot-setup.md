---
# required metadata

title: Set up Intune for Education devices with Windows Autopilot
titleSuffix: Intune for Education
description: Learn how to set up and deploy devices in Intune for Education with Windows Autopilot.  
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 10/24/2019  
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: madakeva  
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Set up devices with Windows Autopilot and Intune for Education  
Windows Autopilot is a cloud-based provisioning technology that can be used in schools to set up and pre-configure new devices, getting them ready for productive use during the school year. Windows Autopilot was designed with school IT departments in mind and provides:   

Easy device setup: Students power on their each devices, connect them to the internet, and sign in. Windows Autopilot automatically configures each device from the cloud and gets them ready for the classroom.  

Time and cost savings in large-scale deployments: Students and teachers can provision devices themselves. IT departments no longer need to set up provisioning in large warehouses and hire a fleet of technicians to set up student PCs.  

Always up to date: Custom images and provisioning packages on USBs can quickly become outdated. With Windows Autopilot, student PCs always get configured with the latest Intune policies and apps.  

Easy reset: Initiate a remote Autopilot Reset from Intune for Education to quickly reset student PCs that are having issues. During a reset, all apps, settings, and user data are removed, while the devices remain enrolled in Azure AD and Intune. After wiping, student PCs automatically receive the latest Intune policies to get them ready for the classroom again. 

## Prerequisites 
Complete these requirements before you begin Windows Autopilot setup in Intune for Education. 

* Determine user permissions: During registration, a [Microsoft partner](https://partner.microsoft.com/) will assign group tags to your devices. If you require different user permissions on different devices, instruct your partner to split the devices in to two group tags, according to permissions. Provide names for each group. For example, if teachers are given admin permissions on your devices and students aren’t, you’d want one group named Contoso Teachers, and another named Contoso Students.  

* Order and register your devices: After you or the Microsoft partner orders the devices from the OEM provider, register the devices for the Autopilot service. We recommend that you connect with a Microsoft partner through [Microsoft Partner Center](https://partner.microsoft.com) and work with them to register the devices. The partner will obtain a CSV with the devices’ information from the OEM and then upload it to Partner Center. For detailed registration instructions, see [Adding devices to Windows Autopilot]( https://docs.microsoft.com/ windows/deployment/windows-autopilot/add-devices). 






## Next steps
[Manage devices with remote actions](edu-device-remote-actions.md)



