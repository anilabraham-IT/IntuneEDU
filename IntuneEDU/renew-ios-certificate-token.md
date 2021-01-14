---
# required metadata

title: Renew iOS certificates and tokens 
titleSuffix: Intune for Education
description: Learn how to renew expired certificates or tokens in the Intune for Education portal.
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
#ms.reviewer: travisj
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Renew iOS certificate and tokens
Apple MDM Push certificates, enrollment program tokens, and VPP tokens expire 365 days after you create them. Intune for Education will alert you when a certificate or token is close to or past its expiration date. 

Make sure to renew them to maintain the connection between your Intune for Education account and Apple account.  

## Renew Apple MDM certificate  
> [!IMPORTANT]
> If the Apple MDM certificate expires or is deleted, you will need to reset and re-enroll devices with a new certificate.  

The MDM push certificate is associated with the Apple ID you used to create it. Renew the certificate with this same Apple ID.

1. Go to **Tenant settings** > **MDM push certificate**.  
2. Select **Renew certificate**.
3. Follow the onscreen instructions to renew and download your MDM push certificate in the Apple Push Certificates Portal. Remember to sign in with the Apple ID you used to create your original certificate. After you renew and download the certificate, return to Intune for Education to complete the remaining fields on this screen.  
4. Select **Save**.    

## Renew enrollment program token 

Renew the enrollment program token annually to keep Intune for Education up to date with your school's devices. This process requires you to sign in to Apple School Manager to download the token.  

1. Go to **Tenant settings** > **Enrollment program tokens**.
2. Select the token that you want to renew.
3. Select **Renew token**.
4. Follow the onscreen instructions. Remember, sign in to Apple School Manager with the Apple ID you used to get your original token. After you renew and download the token, return to Intune for Education to complete the remaining fields on this screen. 
5. Select **Save**.   

## Renew VPP token
Renew your VPP tokens annually to make sure your VPP-purchased apps can be viewed and assigned from Intune for Education.  

The VPP token is associated with the Apple ID you used to create it. Renew the token with this same Apple ID.  

1. Go to **Tenant settings** > **VPP tokens**.
2. Find the token that you want to renew. Select the link that's in the **Associated apps** column.  
3. Select **Renew token**.
4. Follow the onscreen instructions to download and renew your token from Apple School Manager. Remember, sign in to Apple School Manager with the Apple ID you used to get your original token. After you renew and download the token, return to Intune for Education to complete the remaining fields on this screen. 
> [!TIP]
> When choosing a region, select where your school's devices are located. 
5. Select **Save**.   

## Next steps
Now that your certificates and tokens are renewed, make sure [your group settings](edit-groups-intune-for-edu.md) are up to date. To see the current status of your groups in Intune, learn how to [view reports](what-are-reports.md).  

Read [What's new in Intune for Education](whats-new-in-edu.md) to find out about the latest updates and features.