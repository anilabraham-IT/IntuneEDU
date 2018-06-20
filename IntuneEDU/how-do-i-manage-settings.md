---
# required metadata

title: How do I manage settings?
titleSuffix: Intune for Education
description: Follow these steps to manage settings through Intune for Education policies.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 01/17/2018
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

You can manage a variety of settings for your users, apps, and devices with Intune. It is how you will change how devices can respond to user actions.

When settings are applied to a group of devices, users are affected when they access a device from that group. If a setting is applied to a group of users,

Device settings apply to all devices in their group. Settings that are **Not configured** allow the user to define their settings on their devices themselves.

## Manage settings for groups

Use the following steps to manage the full list of settings in Intune for Education:
1. In the [Intune for Education](https://intuneeducation.portal.azure.com) console, in the left-side navigation menu, choose **Groups**.
2. Select the group whose settings you want to manage. For a complete list, see [Available settings](what-are-settings.md).
3. Click **Settings** at the top of the page to view the full list of available settings.
4. Expand categories and modify individual settings for the selected group.
5. Click **Save** to save the changes for that group. Settings are automatically sent to devices in that group.

## Manage settings with Express Configuration

Express Configuration makes it easy for you to get started quickly, but can also help you make quick changes to your devices.

  ![Express Configuration settings fix](./media/express-config-006-choose-settings.png)

1. In the [Intune for Education](https://intuneeducation.portal.azure.com) console, choose **Launch Express Configuration**. Review the **Welcome** page and choose **Get started**.
2. Review the **Get school information** page. If you've already added school information, choose **Next**.
3. Select the group whose settings you want to manage, and then choose **Next**.
4. Review the list of apps, and then choose **Next**.
5. On the **Settings** page, expand the categories of available settings:
   * [Basic device settings](available-settings.md#basic-device-settings)
   * [Microsoft Edge settings](available-settings.md#microsoft-edge-settings)
   * [Device update settings](available-settings.md#device-update-settings)
   * [Wireless settings](available-settings.md#wireless-settings)
   * [App settings](available-settings.md#app-settings)
   * [Sign in settings](available-settings.md#sign-in-settings)

   Expand a category and toggle the control to modify settings, and then choose **Next**.

6. Review your choices and then choose **Finish** to save your changes update them on devices in the selected group.

## Can I ever have settings that don't work together?

It is possible for incompatible settings to be applied to the same group. These inconsistences result in errors, when a user or device is being set up with different settings in multiple places. This happens as a result of the user or device being a member of multiple groups.

For example, Esperanza is a member of the *6th Grade* group and is also a member of group called *Earth Science*. If you configure a homepage setting and assign to *6th Grade*, and you configure a different homepage setting and assign it to *Earth Science*, she now has two conflicting homepage settings assigned to her user. That results in inconsistent settings assignment leading to an error. You can find which devices and users have settings errors using the [settings errors report](what-are-reports.md).

## Find out more

- [Find out more about the full policy management experience in  Intune](https://docs.microsoft.com/intune/deploy-use/manage-settings-and-features-on-your-devices-with-microsoft-intune-policies)
