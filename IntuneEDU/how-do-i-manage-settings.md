---
# required metadata

title: How do I manage settings?
titleSuffix: Intune for Education
description: Follow these steps to manage settings through Intune for Education policies.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 05/06/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 20c0f6c9-f1de-4048-aa96-5b0a068c1b75
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: rashok
#ms.suite: ems
.md#ms.tgt_pltfrm:
#ms.custom: intune-education


---

# How do I manage settings?

Manage  settings for your users, apps, and devices with Intune. Settings that are applied to a *group of devices* affect how and when users from a group can access a device. Settings that are applied to a *group of users* affect how all devices for the group work. 

When a setting in Intune is marked as **Not configured**, a student can access the setting from their device and set it how they want.

## Manage settings for groups

Complete the following steps to manage all settings in Intune for Education:
1. In [Intune for Education](https://intuneeducation.portal.azure.com), go to the left-side navigation menu and choose **Groups**.
2. Select the group whose settings you want to manage. For a complete list, see [Available settings](what-are-settings.md).
3. Click **Settings** to view the full list of available settings.
4. Expand the categories to select and edit individual settings for the selected group.
5. Click **Save** to save the changes for that group. Settings are automatically sent to devices in that group.

## Manage settings with Express Configuration

Express Configuration enables you to get started in Intune quickly. You can also use it at any time to make quick changes to your settings. Complete the following steps to modify settings with Express Configuration.

  ![Express Configuration settings fix](./media/express-config-006-choose-settings.png)

1. In [Intune for Education](https://intuneeducation.portal.azure.com), choose **Launch Express Configuration**. 
2. Review the **Welcome** page and click **Get started**.
2. Review the **Get school information** page. If you've already added school information, click **Next**.
3. Select the group whose settings you want to manage. Then click **Next**.
4. Review the list of apps. Then click **Next**.
5. On the **Settings** page, expand the categories to see all available settings. Toggle the controls to modify settings.
   * [Basic device settings](available-settings.md#basic-device-settings)
   * [Microsoft Edge settings](available-settings.md#microsoft-edge-settings)
   * [Device update settings](available-settings.md#device-update-settings)
   * [Wireless settings](available-settings.md#wireless-settings)
   * [App settings](available-settings.md#app-settings)
   * [Sign in settings](available-settings.md#sign-in-settings)

6. When you are done editing your settings, click **Next**.
7. Review your choices. Click **Finish** to save your changes.

## Confliciting settings in Intune for Education

It is possible to apply conflicting settings in the same group. When an attempt is made to apply these settings to a device or user, an error may occur. Errors are the result of the user or device being a member of multiple groups that have conflicting settings.

For example, Esperanza is a member of the *6th Grade* group and is also a member of group called *Earth Science*. If you configure a homepage setting and assign to *6th Grade*, and you configure a different homepage setting and assign it to *Earth Science*, she now has two conflicting homepage settings assigned to her. When you try to assign the settings to her, you'll receive an error. For more information about devices and users with settings errors see [settings errors report](what-are-reports.md).

## Find out more

- [Find out more about the full policy management experience in  Intune](https://docs.microsoft.com/intune/deploy-use/manage-settings-and-features-on-your-devices-with-microsoft-intune-policies)