---
# required metadata

title: Set up iOS device management
titleSuffix: Intune for Education
description: Enable iOS device management to sync and manage iOS devices from the Intune for Education portal.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 01/14/2021
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.subservice: education
ms.technology:
ms.assetid: c884df47-61a9-4799-a407-8cd311d376d1
searchScope:
 - IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: elcox
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Set up iOS device management 

Before you can manage or assign iOS devices to students and teachers, you must set up iOS device management in Intune for Education. Setup requires you to add an MDM Push Certificate and configure at least one enrollment program token (also known as an MDM server token or DEP token).  

  [![Screenshot of the Tenant Settings, iOS Device Management Overview page, showing 3 interactive cards in a row named Set up MDM push certificate, Set up enrollment program token, and Set up Volume Purchase Program (VPP) token. Each card has a "Configure" or "Manage" button for users to begin setup or edit existing configurations.](./media/set-up-ios-management-landing-2101.png)](./media/set-up-ios-management-landing-2101.png#lightbox)   

During setup, you'll connect your Intune for Education account with your Apple School Manager account. The connection makes sure that Intune for Education always has the most current details about your purchased iOS devices.  

This article describes how to:

* Add an Apple MDM push certificate.
* Configure and sync an enrollment program token.
* Configure an Apple VPP token.  

## What happens after I set up device management?
After you set up iOS device management, you can use Intune for Education to manage apps and settings on your iOS devices. You'll also have access to reports and actions so you can troubleshoot conflicts anywhere.  

Students and teachers in your school will be able to securely access school websites and email.  

## Requirements
Before beginning, make sure you have:  
* An internet connection.
* Your Apple School Manager account credentials.
* Intune for Education device licenses. Find out more about the device licenses in the [Intune licenses docs](https://docs.microsoft.com/mem/intune/fundamentals/licenses).  

> [!IMPORTANT]
> Intune for Education only supports iOS device enrollment for devices bought through Apple Automated Device Enrollment. For more information about Automated Device enrollment and Apple School Manager, see the [Apple automated device enrollment support site](https://go.microsoft.com/fwlink/?linkid=2142075&clcid=0x409).  

## Add an MDM push certificate
An Apple MDM push certificate sets up a secure connection between your Intune and Apple School Manager account. When connected, Intune can continually sync and manage your Apple devices and apps. 

1. Sign in to Intune for Education.  
2. Go to **Tenant settings** > **MDM push certificate**.
3. Select **Create certificate**.   
4. Follow the onscreen instructions:   
    1. Select **Download** to save the certificate signing request file from Intune. 
    2. Sign in to Apple Push Certificates Portal to create and download the push certificate. Use your school's Apple ID to sign in, not your personal one.  
    3. Return to the Intune for Education portal and enter the Apple ID you used to sign in to Apple School Manager.
    4. Upload the Apple push certificate file.  
5. Select **Save** to create the certificate in Intune for Education.  

The push certificate expires every 365 days. The certificate is needed to connect Intune for Education to your Apple School Manager account, so [you'll need to renew it yearly](renew-ios-certificate-token.md).  


## Configure enrollment program token  
Sometimes referred to as a DEP token or MDM server token, the enrollment program token lets Intune sync device details from Apple School Manager. These details inform Intune of the devices it needs to manage, and populates your inventory in the Intune for Education portal.  

### Shared iPad configuration  
You can configure your iOS devices to enroll as Shared iPad devices. With Shared iPad, students and teachers sign in to your school's devices with their unique Managed Apple ID. As they move from device to device, their apps and data move with them. A student can use one device to begin writing a paper, and then sign in to a different device later to finish the paper. To learn more about *Shared iPad* and *Managed Apple IDs*, visit the [Apple Education website](https://www.apple.com/education/it/) and [documentation](https://go.microsoft.com/fwlink/?linkid=2060097&clcid=0x409).  

Classroom devices can still be shared between students, even without Shared iPad. However, user data doesn't move between devices. Before you configure your server token, you'll choose if you want to enable Shared iPad. 

> [!NOTE]
> If you set up a device with Shared iPad, you'll get all of features that come with Shared iPad, except for the Classroom and Schoolwork apps. These apps aren't supported by Intune for Education. Shared iPad features will become available after you set up the enrollment program token.  

### Add enrollment program token  

The following steps describe how to add an enrollment program token to Intune for Education.  

1. Go to **Tenant Settings** > **Enrollment program tokens**.
2. Select **Add token**.
3. Choose how you want to enroll the devices associated with your new server token. This option can't be changed once the token is created. If you want to change how devices enroll later, you'll need to create a new server token. 
    * To configure this token for Shared iPad, choose **Users will log in to devices with their Managed Apple IDs**. All devices assigned to this token will be set up so that users must sign in to them with a Managed Apple ID.  
    * If your school isn't using Managed Apple IDs, choose **Anyone can unlock these devices...** Devices can still be shared by students but they'll be accessed directly, without the need to sign in. They might require a device passcode if you set one.  

4. Select **Set up enrollment program token**.  
5. Follow the onscreen instructions:  
    1. Choose a device name prefix.  
    2. Select **Download** to save the Intune public key so that you can upload it later.  
    3. Sign in to Apple School Manager to create and download a token. Use your school's Apple ID to sign in, not your personal one. If you don't have the MDM server information to complete this step, contact your school's Intune administrator.  
    4. Stay in Apple School Manager and go to **Device Assignments**. Enter the serial number for each device, the order number for your entire device purchase, or a list of your devices in a CSV file.  From the drop-down menu, select **Assign to Server**. Then choose the MDM server you just created.  
    5. Return to Intune for Education and enter the Apple ID you used to sign in to Apple School Manager.  
    6. Upload the enrollment program token.  
6. Select **Save** to add the token to Intune.  

Enrollment program tokens expire every 365 days. The token is needed to view and manage your devices in the Intune for Education portal. You'll need to [renew it yearly](renew-ios-certificate-token.md).

### Device enrollment profile
Intune for Education creates and applies an iOS enrollment profile to each enrollment profile you configure.

All iOS devices added to Intune for Education are set to supervised mode. As an admin, supervised mode allows you more control over your school's devices. For example, you can push new apps or app updates silently to a device. For a complete list of supervised-only settings, see the article, [Configurations requiring supervision](/intune/device-restrictions-ios#settings-that-require-supervised-mode).

Intune for Education applies a naming scheme to devices that you enroll with an enrollment program token. The name will help you identify and group individual devices. By default, devices are named with their device serial number. You can also add on a custom device name when you set up your enrollment program token.  

For more details about enrollment profiles, view the [list of settings configured](add-devices-ios-edu.md#preconfigured-settings) during enrollment.  

### Sync managed devices
Now that Intune for Education has permission to manage your iOS devices, sync with Apple to view a list of your managed devices.    

1. Go to **Enrollment program tokens** to find the token you created. Select the link that's under the **Devices ready to enroll** column in the same row.  
2. Select **Sync device list**. 

Devices that appear in the list are ready for enrollment. Power them on to start the enrollment process. 

## Configure VPP tokens

 A VPP token links your Intune for Education account to your Apple VPP or Apple School Manager account. You can create a single VPP token to manage apps across the entire organization; or you can create multiple VPP tokens to spread management across different locations or admins.  

VPP tokens are necessary for Intune to:  
* Sync app details in the Intune for Education portal.
* Assign VPP-purchased apps to groups.
* Silently install VPP-purchased apps on school devices, with no need for device user's Apple ID.

Without a VPP token, you can still search and get [free iOS apps through the App Store](add-apps-ios.md). However, to install the app on the device, the device user must sign in with an Apple ID. 

1. Go to **Tenant Settings** > **VPP Tokens**.
2. Select **Add token**. 
3. Name the VPP token and then follow the onscreen instructions to create the token:  
    1. Sign in to Apple School Manager to create and download a token. Use your school's Apple ID to sign in, not your personal one. 
    2. Return to the Intune for Education portal and enter the Apple ID you used to sign in to Apple School Manager.
    3. Upload the VPP token file and then select the region where your devices are. 
    4. Enable or disable automatic app updates. 
4. Select **Save** to add the token to Intune.  

Tokens expire every 365 days. Tokens are needed to manage VPP-purchased apps, so [you'll need to renew them yearly](renew-ios-certificate-token.md).  

### What's a managed device?
To help you understand the difference between a managed and unmanaged device, let's look at the following scenario.

A teacher brings a personal iOS device to school. During school hours, the teacher uses the device to schedule parent meetings and track of class assignments.  

 The device wasn't purchased by the school through the Apple DEP program. It's not enrolled under the Intune for Education tenant. As a result, there's no way for Intune to communicate with the teacher's device. The device is considered not managed so the IT admin has no control over how the teacher uses the device during school hours. 

Similarly, since it's not a known managed device, the teacher can't access protected school resources, such as email.  

## Next steps

Purchase [free apps from the App Store](add-apps-ios.md), or [add your VPP-purchased apps](add-vpp-apps-ios.md) to the Intune for Education portal.  

