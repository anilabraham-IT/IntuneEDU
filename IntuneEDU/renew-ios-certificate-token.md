---
# required metadata

title: Renew iOS certificates and tokens 
titleSuffix: Intune for Education
description: Learn how to renew expired certificates or tokens in the Intune for Education portal.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 01/13/2021
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
Apple MDM Push certificates, MDM server tokens, and VPP tokens expire 365 days after you create them. Intune for Education will alert you when a certificate or token is close to or past its expiration date. 

Make sure to renew them to maintain the connection between your Intune for Education account and Apple account.  

## Renew Apple MDM certificate  
> [!IMPORTANT]
> If the Apple MDM certificate expires or is deleted, you will need to reset and re-enroll devices with a new certificate.  

The MDM push certificate is associated with the Apple ID you used to create it. Renew the certificate with this same Apple ID.

1. From the Intune for Education dashboard, select **Tenant settings**.
2. Select **MDM push certificate**.
3. Select **Renew certificate**.
4. Follow the onscreen instructions. You'll be required to visit the Apple Push Certificates portal to renew your MDM push Certificate. Remember, sign in to the Apple Push Certificates portal with the Apple ID you used to create your original certificate.  
    5. When you get to the Apple Push Certificates portal, find the certificate and then select **Renew**.   
    6. Once the certificate is active again in the Apple Push Certificates Portal, select **Download**. Save the certificate file.    
    7. After downloading the file, return to Intune for Education.
    8. Enter your Apple ID and upload the certificate file. 
5. Select **Save**.  

## Renew Enrollment program token

Renew the MDM server token annually to make sure that Intune for Education always has an updated list of your iOS devices.

The MDM server token is associated with the Apple ID you used to add the server. Renew the token with this same Apple ID. 

1. From the Intune for Education dashboard, select **Tenant settings**.
2. Select **Enrollment program tokens**.
3. Select the token that you want to renew.
4. Select **Renew token**.
5. Follow the instructions on the **MDM Server Tokens** page. You'll be required to visit Apple School Manager to generate a new MDM Server Token. Remember, sign in to Apple School Manager with the Apple ID you used to get your original token.
    6. After you download and save the new token from Apple School Manager, return to the Intune for Education portal. 
    7. Enter your Apple ID and upload the token file. 
8. Select **Save**.


## Renew VPP token
Renew your VPP tokens annually to make sure your VPP-purchased apps can be viewed and assigned from Intune for Education.  

The VPP token is associated with the Apple ID you used to create it. Renew the token with this same Apple ID.  

1. From the Intune for Education dashboard, select **Tenant settings**.
2. Select **VPP Tokens**.
2. Find the token that you want to renew. Select the link that's in the **Associated apps** column.  
3. Select **Renew token**.
4. Follow the onscreen instructions to download and renew your token from Apple School Manager. Remember, sign in to Apple School Manager with the Apple ID you used to get your original token.
> [!TIP]
> When choosing a region, select where your school's devices are located. 
10. Select **Save** to finish with the token.  

## Next steps
Now that your certificates and tokens are renewed, make sure [your group settings](edit-groups-intune-for-edu.md) are up-to-date. To see the current status of your groups in Intune, learn how to [view reports](what-are-reports.md).  

Read [What's new in Intune for Education](whats-new-in-edu.md) to find out about the latest updates and features.