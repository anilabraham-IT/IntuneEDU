---
# required metadata

title: Renew Apple MDM certificate
titleSuffix: Intune for Education
description: Learn how to renew expired certificates or tokens in the Intune for Education portal.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/03/2018
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

# Renew iOS certificate and tokens
Apple MDM push certificates, MDM server tokens, and VPP tokens expire 365 days after you create them. Intune for Education will alert you when a certificate or token is close to or past its expiration date. Make sure to renew them to maintain the connection between your Intune for Education account and Apple account.

## Renew Apple MDM push certificate
The Apple MDM push certificate is valid for 365 days from the date you create it. Renew it annually to maintain iOS device management in Intune for Education. 

The MDM push certificate is associated with the Apple ID you used to create it. Renew the certificate with this same Apple ID.

1. From the Intune for Education dashboard, click **Tenant settings** > **iOS Device Management**.
2. On the **iOS Device Management** page, click the **MDM Push Certificate** tab.
3. Click **Renew certificate**.
4. Follow the instructions on the **MDM Push Certificate** page. You'll be required to visit the Apple Push Certificate portal to renew your MDM push Certificate. Remember, sign in to the Apple Push Certificates portal with the Apple ID you used to create your original certificate.
5. When you're in the Apple Push Certificate portal, click the option to renew the expiring certificate. Complete the steps in the Apple portal. When your certificate's status reads **Active** again, click to download and save it.
6. Return to the Intune for Education portal and upload the certificate. 
7. Click **Save**.

## Renew MDM server token

The MDM server token is valid 365 days from when you create it. Renew it annually to maintain an updated list of iOS devices in Intune for Education. 

The MDM server token is associated with the Apple ID you used to add the server. Renew the token with this same Apple ID. 

1. On the iOS Device Management page, click the **DEP Tokens** tab.
2. Select the token that you want to renew.
3. Click **Renew token**.
4. Follow the instructions on the **MDM Server Token** page. You'll be required to visit Apple School Manager to generate a new MDM Server Token. Remember, sign in to Apple School Manager with the Apple ID you used to get your original token.
5. After you download and save the new token from Apple School Manager, return to the Intune for Education portal. Type in the Apple ID used to create the original token.
6. Upload the token that you downloaded and saved.
7. Click **Save**.


## Renew VPP token

## Next steps