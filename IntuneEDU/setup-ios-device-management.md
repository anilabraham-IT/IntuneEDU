---
# required metadata

title: Set up iOS device management
titleSuffix: Intune for Education
description: Enable iOS device management to sync and manage iOS devices from the Intune for Education portal.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 05/10/2017
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

# Configure iOS device management 

 Intune for Education supports device management for iOS devices purchased through the Apple device enrollment program (DEP). When enabled, students can securely access school resources from your managed iOS devices. As an admin, it lets you modify device and app use, groups, wi-fi profiles, and tenant settings. You'll also have access to reports and actions so you can troubleshoot conflicts from a far. 

Until a device is enrolled in management, you as an admin can't modify its settings through the Intune for Education portal. This article describes how to enable iOS device management so that devices can start enrolling in Intune management. By the end of this article you'll know how to:

* Upload an Apple MDM Push certificate
* Upload Apple DEP tokens
* Upload Apple VPP tokens

During setup make sure you have:
* Access to the Internet.
* Your Apple School Manager account credentials
* Intune for Education device licenses. Find out more about the device licenses in the [licenses docs](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune-step-4)

> [!IMPORTANT]
> Intune for Education only supports iOS device enrollment for devices bought through Apple DEP. If you did not buy a device through an approved Apple DEP vendor, you must manually enter the device serial number into Apple School Manager. For more information about Apple School Manager, see <link>.

## Education-optimized settings for iOS devices
When you turn on a managed device for the first time, Intune for Education applies a pre-configured iOS profile. The profile is made up of school-specific, Microsoft-recommended settings that support classroom productivity and student focus. 

All iOS devices added to Intune for Education are set to supervised mode. As an admin, this allows you more control over your school's devices, such as being able to push new apps or app updates silently to a device.  For a complete list of supervised-only settings, see the article, [Configurations requiring supervision](https://docs.microsoft.com/en-us/intune/device-restrictions-ios#configurations-requiring-supervision).


### What's a managed device?
The following scenario describes the difference between a managed and unmanaged device.

A teacher brings a personal iOS device to school. During school hours, the teacher uses the device to schedule parent meetings and to keep track of class assignments. The device wasn't purchased by the school through the Apple DEP program. It's not enrolled under the Intune for Education tenant. As a result,there's no way for Intune to communicate with the teacher's device. The device is considered not managed -- the IT admin has no control over how the teacher uses the device during school hours. 

Similarly, since it's not a known, managed device, the teacher won't be able to access protected school resources, such as email.


## Upload an MDM Push certificate
An Apple MDM push certificate sets up a secure connection between your Intune and Apple School Manager account. It ensures that Intune can continually sync and manage the device and apps you set up with Apple. 

1. Sign in to the Intune for Education Portal.
2. Click **Tenant settings** > **iOS device management**.
3. On the **iOS Device Management** page, click the **MDM Push Certificate** tab.
4. Follow the instructions on the **MDM Push Certificate** page. You are required to visit the Apple Push Certificate portal to create an MDM Push Certificate. Sign in to the Apple Push Certificates portal with your school's Apple ID, not your personal one.
5. Read and acknowledge the consent agreement at the bottom of the page.
6. Click **Save**.

The push certificate expires every 365 days. The certificate is essential to connecting Intune to your Apple School Manager account, so you'll need to renew it yearly. <link to article>

## Configure MDM server tokens
Sometimes referred to as a DEP token, the MDM server token lets Intune sync device details from Apple School Manager. These details inform Intune of the devices it needs to manage, and populate your inventory in the Intune for Education portal. The MDM server token also permits Intune to upload pre-configured device enrollment profiles.<link to article about default settings>

1. On the iOS Device Management page, click the **DEP Tokens** tab.
2. Click **Set up token**.
3. Click **Download** to download the required Intune public key. This file will be used to request the trusted certificate from Apple School Manager. Save the file to your computer.
4. Click **Go to my MDM Servers in Apple School Manager." 
5. If prompted, sign in to Apple School Manager with your school's Apple ID, not your personal one. 
6. Go the MDM servers section of the site and click the option to add a new MDM server.
7. Follow the steps on screen to generate a server token. Then save your changes. If you don't have the information to complete this step, contact your school's Intune administrator. 
8. Remain in Apple School Manager and go to the device assignments page. Enter the serial number for each device, the order number for your entire device purchase, or a list of your devices in a CSV file. 
9. Select the option to assign your devices to the MDM server.
10. Return to the Intune for Education portal and enter the Apple ID you used to sign in to the Apple Push Certificates portal.
11. Upload the MDM server token that you created in step 7 of this procedure. 
12. Read and acknowledge the consent agreement at the bottom of the page.
13. Click **Save**.

Tokens expire every 365 days. The token is essential to viewing and managing your devices in the Intune for Education portal. You must renew it yearly. <link to article>

## Configure VPP tokens

 //lenewsad I'm seeing multiple tokens in the Intune for EDU console. Why is that? In a typical school, will they have multiple tokens, or are they restricted to just one?
//lenewsad How many VPP tokens can a tenant have?

VPP token should be set up per it admin or per school. Location = VPP token. So you cacn assign 100 snapchat licenses to 

 A VPP token links your Intune for Education account to your Apple VPP or Apple School Manager account. VPP tokens are necessary for Intune to:
* Sync app details in the Intune for Education portal
* Assign VPP-purchased apps to groups 
* Silently install VPP-purchased apps on school devices, with no need for device user's Apple ID

Without a VPP token, you can still search and get free iOS apps through the App Store. However, to install the app on the device, the device user must sign in with an Apple ID. 

1. On the iOS Device Management page, click the **VPP Tokens** tab.
2. Click **Open Apple School Manager** and sign in with your school's Apple ID, not your personal one. If you use the legacy Apple VPP site to buy apps, click **Download your token from the VPP website**. Follow the steps on the sites to create and download the token. Save the token to your local drive.
3. Return to the Intune for Education portal. Enter the Apple ID that you used to sign in to the Apple Push Certificates portal.
4. Click the folder icon to browse your computer's files. Select the token file that you downloaded and saved in step 2.
5. Choose the location of your school's devices. //lenewsad is this accurate? the location of the app store.
6. //lenewsad Looks like the up-to-date setting is enabled by default? Switch the setting to disable automatic app updates.  *might remove from steps due to engineering
7. Read and acknowledge the consent agreement at the bottom of the page.
8. Click **Save**.

You can create a single VPP token to manage apps across the entire organization; or you can create multiple VPP tokens to designate app management among different locations or admins in your organization.

Tokens expire every 365 days. (//lenewsad: what about password reset? TBD. Ravi is checking on this.) Tokens are essential to managing VPP-purchased apps, so you'll need to renew them yearly. <link to article>

## Next steps
* Add iOS apps in Intune 
* Add VPP-purchased apps in Intune

