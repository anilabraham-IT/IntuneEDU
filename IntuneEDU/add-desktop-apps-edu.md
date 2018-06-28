---
# required metadata

title: Add desktop apps to Intune for Education
titleSuffix: Intune for Education
description: Learn how to upload and add new desktop app files to Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/27/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 24ab6547-aa65-428a-b184-06b806e95bd1
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

# Add desktop apps to Intune for Education

Upload and add desktop apps to your Intune for Education app list. After you've added the apps, you can [assign them to groups](install-apps.md) and install them on school devices. 

To complete these steps, you will need the installation file for the app that you want to add.

1. Sign in to the Intune for Education portal.
2. Click **Apps**.
3. In the left pane of the blade, under **DESKTOP APPS**, click **New app**.
4. In the **New desktop app** section, enter the following details:
   * **App file** — Upload an MSI installer for the app.
   * **App name** — The name of the app to appear on devices.
   * **Description** — A description of the app that will help you quickly identify it.
   * **Publisher** — The name of the app publisher, to help you quickly identify the app developer.
   * **Icon** — Upload a PNG or JPG file to use as the app's icon.
5. Click the folder icon and select the app installation file from your computer. 
6. Click **Save**. The app will then upload to Intune for Education. Once the upload is complete, you can [assign the app to devices](install-apps.md). 

   ![The add new desktop app screen, with all fields filled out for sample app, evernote.](./media/apps-004-filled-out-desktop-app.png)  

> [!NOTE]
> If you run into the error, "The app doesn't have an install file" or "No app install file was added," the file didn't upload properly. To fix this, try to upload and save the file again.
