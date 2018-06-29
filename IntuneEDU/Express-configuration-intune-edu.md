---
# required metadata

title: Express Configuration
titleSuffix: Intune for Education
description: Use Express Configuration to set up your groups in Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/25/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: af5d35ee-84f5-4245-a441-671600bcc376
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

# Express Configuration in Intune for Education

  ![The Express Configuration tile, which says Launch Express Configuration, Click here to choose apps and settings for a group.](./media/express-config-001-launch-tile.png)

Express Configuration enables you to assign settings and apps to users and devices. The launch tile for the step-by-step walkthrough is found on the front page of the [Intune for Education portal](https://intuneeducation.portal.azure.com). 

As you click through each step, you'll see that most of the Windows or iOS settings are already configured. These configurations are the default values and are set as recommendations. Recommended OS-specific apps are also preselected. Change the default selections as needed for your school. 

Return to Express Configuration anytime you want to make changes to a group's settings or apps. 

## Launch Express Configuration
This section describes how to complete the steps in Express Configuration. To get the most out of the Express Configuration, make sure you've synced your school data or created groups in Azure AD. 

1. Sign in to the Intune for Education portal.
2. On the dashboard, click **Launch Express Configuration**.

If iOS configurations are disabled when you launch Express Configurations:
1. From the dashboard select **See all** > **iOS device management**.
2. Upload an Apple MDM Push Certificaate.
3. Register an [Apple Device Enrollment Program (DEP) token](setup-ios-device-management.md).

## Choose a group to configure

Default groups are included with your Intune for Education subscription. They are populated with the details of your school records. Default groups include:  
    * All Devices
    * All Users
If you used SDS to import your school's records, you'll also see:      
    * All Teachers
    * All Students 

We recommend that you start with the **All Users** group, and assign the settings that all users must have. For example, assign settings such as password requirements or pop-up restrictions in Microsoft Edge.

  ![The choose group screen, which asks users to select a group.](./media/express-config-004-choose-group.png)

Click the expand/collapse arrow to view or hide all groups. Remember, if you configure a top-level group, all settings you apply to that group will be inherited by its subgroups.

## Choose apps

The types of apps that you can provision to devices include:
* [Web apps](add-web-apps-edu.md)
* Windows 10 apps
    * Microsoft Office
    * [Microsoft Store for Education apps](acquire-store-apps.md)
    * [Desktop apps](add-desktop-apps-edu.md)
* [iOS apps]
    * [Free iOS App Store apps](add-apps-ios.md)
    * [Volume purchased program (VPP) apps](add-vpp-apps-ios.md)

Select one or more apps to assign. Apps will be immediately assigned to your group after you click **Next**.

  ![The app assignment screen. Apps are organized for assignment by different types, including web apps and Microsoft Store for Education apps.](./media/express-config-005-choose-apps.png)

Intune for Education also displays [popular apps from the Microsoft Store for Education](add-popular-apps-edu.md) from across all Intune for Education users.


## Choose settings
Express Configuration shows you common settings for devices and users in Intune. Settings are separated into OS-specific categories: Windows settings and iOS settings.

The default settings are preset with recommended values. If you want to stick with the recommendations, and not make any changes, click **Next**. Settings will immediately be applied to your group. 

  ![The choose settings screen. Settings are organized into a collapsed list, including divisions such as device sharing, basic device settings, app settings, browser settings, and more.](./media/express-config-006-choose-settings.png)


Change Express Configuration selections at any time to fit your school's changing policies. For even more customization capabilities in Intune for Education, view the full list of [Windows 10](edu-settings-windows.md) and [iOS](edu-settings-ios.md) device settings.

## Review settings

Before saving, review your apps and settings selections. Click **Back** to make changes. When your review is complete, click **Save**.

  Not up to date: ![The review your choices screen. It shows the apps and settings selected during Express Configuration.](./media/express-config-007-save-changes.png)  

  ![The completion screen. It shows the configure more groups and completed options. The All Done option offers a short explanation of what's next in the process, including adding devices to Intune for Education by joining them to Azure Active Directory.](./media/express-config-008-all-done.png)

## Next steps

