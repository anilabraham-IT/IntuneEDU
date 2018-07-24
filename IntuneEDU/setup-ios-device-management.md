---
# required metadata

title: Set up iOS device management
titleSuffix: Intune for Education
description: Enable iOS device management to sync and manage iOS devices from the Intune for Education portal.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
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

# Setup iOS device management 

Before you can manage or assign iOS devices to students and teachers, you must set up iOS device management in Intune for Education. This setup requires that you add an MDM Push Certificate and configure at least one MDM Server Token (also known as a DEP token).  

  ![Screenshot of the Tenant Settings, iOS Device Management page, showing green circles with white checkmarks on the MDM Push Certificate, MDM Server token, and VPP token cards. Circles indicates that all are configured. User can click the blue rectangular button that says "Manage" to edit or update configurations.](./media/set-up-ios-management-landing-1807.png)   

During setup, you'll connect your Intune for Education account with your Apple School Manager account. The connection makes sure that Intune for Education always has the most current details about your purchased iOS devices.

This article describes how to:

* Add an Apple MDM Push certificate.
* Configure and sync an Apple MDM Server token.
* Configure an Apple VPP token.

## What happens after I setup device management?
After you've set up iOS device management, you'll be able to use Intune for Education to manage apps and settings on your iOS devices. You'll also have access to reports and actions so you can troubleshoot conflicts anywhere.  

Students and teachers in your school will be able to securely access school websites and email.  

## Requirements
Before beginning, make sure you have:  
* An internet connection.
* Your Apple School Manager account credentials.
* Intune for Education device licenses. Find out more about the device licenses in the [Intune licenses docs](https://docs.microsoft.com/intune/get-started/start-with-a-paid-subscription-to-microsoft-intune-step-4).  

> [!IMPORTANT]
> Intune for Education only supports iOS device enrollment for devices bought through Apple DEP. For more information about Apple School Manager, see the [Apple education support site](https://support.apple.com/education).  

## Add an MDM Push certificate
An Apple MDM Push certificate sets up a secure connection between your Intune and Apple School Manager account. When connected, Intune can continually sync and manage your Apple devices and apps. 

1. Sign in to the Intune for Education Portal.
2. Go to the sidebar and click **Tenant settings** > **iOS Device Management**.
3. Click the **MDM Push Certificate** tab.
4. Follow the instructions on the **MDM Push Certificate** page. You will be required to visit the Apple Push Certificates portal to create an MDM push certificate. Sign in to the Apple Push Certificates portal with your school's Apple ID, not your personal one.
5. Complete the steps in the Apple portal. After you create the certificate, click to download and save it.
6. Return to the Intune for Education portal and enter the Apple ID you used to sign in to Apple Push Certificates portal.
7. Upload the certificate you downloaded.
8. Click **Save**.  

The push certificate expires every 365 days. The certificate is needed to connect Intune for Education to your Apple School Manager account, so [you'll need to renew it yearly](renew-ios-certificate-token.md).  


## Configure MDM server tokens  
Sometimes referred to as a DEP token, the MDM server token lets Intune sync device details from Apple School Manager. These details inform Intune of the devices it needs to manage, and populate your inventory in the Intune for Education portal.  

1. On the **iOS Device Management** page, click the **MDM Server Tokens** tab.
2. Click **Set up token**.
3. Click **Download** to download the required Intune public key. You'll need to upload this file in Apple School Manager to create your MDM server token. Save the file to your computer.
4. Click **Go to my MDM Servers in Apple School Manager**. If prompted, sign in to Apple School Manager with your school's Apple ID, not your personal one.
5. Follow the steps on screen to create an MDM server. Then save your changes. If you don't have the information to complete this step, contact your school's Intune administrator.
6. Download and save the token for the MDM server.
7. Stay in Apple School Manager and go **Device Assignments**. Enter the serial number for each device, the order number for your entire device purchase, or a list of your devices in a CSV file. 
  ![Screenshot of the Apple School Manager website, Device Assignments page. Shows step 1, "Choose Devices" with radio button selections and an empty field box for user to enter how they want to manually input purchased devices. Shows step 2, "Choose Action" with a drop-down menu where user should select "Assign to Server."](./media/Apple-School-Manager-MDM-Server-token-1807.png)   
1. From the drop-down menu, choose **Assign to Server**. Then choose the MDM server you just created.
2. Return to the Intune for Education portal and enter the Apple ID you used to sign in to Apple School Manager.
3. Upload the MDM server token you downloaded.
4. Click **Save**.

MDM server tokens expire every 365 days. The token is needed to view and manage your devices in the Intune for Education portal. You'll need to [renew it yearly](renew-ios-certificate-token.md).

### Device enrollment profile
Intune for Education creates and applies an iOS enrollment profile to each MDM server token you configure.

All iOS devices added to Intune for Education are set to supervised mode. As an admin, supervised mode allows you more control over your school's devices. For example, you can push new apps or app updates silently to a device. For a complete list of supervised-only settings, see the article, [Configurations requiring supervision](https://docs.microsoft.com/en-us/intune/device-restrictions-ios#configurations-requiring-supervision).  

For more details about enrollment profiles, view the [list of settings configured](add-devices-ios-edu.md#list-of-preconfigured-settings) during enrollment.

### Sync managed devices
Now that Intune for Education has permission to manage your iOS devices, sync with Apple to view a list of your managed devices.  
1. Sign in to Intune for Education.
2. Click **Tenant settings** > **iOS Device Management** > **DEP Tokens**.
3. Click on any of the listed tokens.
4. Click **Sync device list**. 

Devices that appear in the list are ready for enrollment. Power them on to start the enrollment process.

## Configure VPP tokens

 A VPP token links your Intune for Education account to your Apple VPP or Apple School Manager account. You can create a single VPP token to manage apps across the entire organization; or you can create multiple VPP tokens to spread management across different locations or admins.  

VPP tokens are necessary for Intune to:  
* Sync app details in the Intune for Education portal.
* Assign VPP-purchased apps to groups.
* Silently install VPP-purchased apps on school devices, with no need for device user's Apple ID.

Without a VPP token, you can still search and get [free iOS apps through the App Store](add-apps-ios.md). However, to install the app on the device, the device user must sign in with an Apple ID. 

1. On the **iOS Device Management** page, click the **VPP Tokens** tab.
2. Click **Open Apple School Manager** and sign in with your school's Apple ID, not your personal one.
3. Follow the steps in Apple School Manage to create and download the token. Save the token to your local drive.
4. Return to the Intune for Education portal. Enter the Apple ID that you used to sign in to Apple School Manager.
5. Click the folder icon to browse your computer's files. Select the token file that you downloaded and saved earlier.
6. Choose the location of your school's devices.
7. If you don't want to enable automatic app updates, switch the setting to disable them. 
8. Click **Save**.

Tokens expire every 365 days. Tokens are needed to manage VPP-purchased apps, so [you'll need to renew them yearly](renew-ios-certificate-token.md).

### What's a managed device?
To help you understand the difference between a managed and unmanaged device, let's look at the following scenario.

A teacher brings a personal iOS device to school. During school hours, the teacher uses the device to schedule parent meetings and to keep track of class assignments.  

 The device wasn't purchased by the school through the Apple DEP program. It's not enrolled under the Intune for Education tenant. As a result, there's no way for Intune to communicate with the teacher's device. The device is considered not managed -- the IT admin has no control over how the teacher uses the device during school hours. 

Similarly, since it's not a known, managed device, the teacher won't be able to access protected school resources, such as email.  

## Next steps

Purchase [free apps from the App Store](add-apps-ios.md), or [add your VPP-purchased apps](add-vpp-apps-ios.md) to the Intune for Education portal.  

