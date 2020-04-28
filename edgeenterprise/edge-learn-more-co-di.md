---
title: "ClickOnce and DirectInvoke in Microsoft Edge"
ms.author: kele
author: dan-wesley
manager: srugh
ms.date: 09/16/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Learn about ClickOnce and DirectInvoke in Microsoft Edge."
---

# Understand the ClickOnce and DirectInvoke features in Microsoft Edge

ClickOnce and DirectInvoke are features available in IE and Microsoft Edge (version 45 and earlier) that support the use of a file handler to download files from a website. Although they serve different purposes, both features let websites specify that a file requested for download is passed to a file handler on the user’s device. ClickOnce requests are handled by the native file handler in Windows. DirectInvoke requests are handled by a registered file handler specified by the website hosting the file.

For more information about these features, see:

- [ClickOnce](https://docs.microsoft.com/visualstudio/deployment/clickonce-security-and-deployment?view=vs-2019)
- [DirectInvoke]( https://technet.microsoft.com/learning/jj215788(v=vs.94).aspx)

> [!NOTE]
> Currently, Chromium doesn't provide native support for ClickOnce or DirectInvoke.

## Overview: prerequisites and process

For ClickOnce and DirectInvoke to work as designed and for the file handler to be successfully requested, the file handler must be registered to the operating system as supporting ClickOnce or DirectInvoke. This registration typically happens when the original operating system is installed or when a new program that’s installed requests the ability to use DirectInvoke for updates.

When a website receives a download request that requires ClickOnce or DirectInvoke, the following actions happen:

- The website requests that the browser use a specified file handler.
- The browser checks the operating system registry to see if the file handler is registered for the requested file type.
- If the file handler is registered, the browser calls the file handler and passes the URL as an argument to the file handler.
- The file handler processes the URL and downloads the file.

  > [!NOTE]
  > The URL is used to determine the source of the file, as well as any parameters to use when accessing the file.  For example: endpoints, a manifest, or metadata.

## Use cases

The following use cases are representative.

You can use ClickOnce to easily deploy and update software on devices with minimal user interaction. Users can install and run a Windows application by clicking a link in a web page. If configured correctly, the ClickOnce application can install programs without having users set configurations for the installer. For example, file locations, what options to install, and so on.

DirectInvoke use cases depend on the intent of the website requesting DirectInvoke. For example, the collaborative file-editing feature of Microsoft Word. Instead of clicking a link and downloading the entire copy of a document you’re working on with your colleagues, DirectInvoke lets you download the parts of the document that have been changed. This reduces the amount of data transferred and can reduce the time needed to open the document.  

## Current support for ClickOnce and DirectInvoke in Microsoft Edge

Support for ClickOnce and DirectInvoke:

- DirectInvoke is supported out of the box for all Windows users but ClickOnce is disabled for all Windows users.

  > [!NOTE]
  > Users that need ClickOnce support can go to edge://flags/#edge-click-once and select **Enable** from the dropdown list. You'll have to **Restart** the browser.

- ClickOnce and DirectInvoke aren’t supported on any platforms other than Windows.
- Because ClickOnce is an enterprise-focused feature that’s used by a specific group of power users and not intended for general use, ClickOnce is disabled by default.

## ClickOnce and DirectInvoke file handling security

ClickOnce and DirectInvoke are protected by Microsoft Defender SmartScreen’s URL reputation scanning service.

If a ClickOnce or a DirectInvoke request was is flagged by the Microsoft Defender SmartScreen URL reputation service as unsafe, users with ClickOnce or DirectInvoke enabled will see two popups.

The first popup asks the user if they want to open the file. This popup is displayed regardless of whether the file was flagged as safe or unsafe. The user can **Report the file as unsafe**, **Cancel** the request, or click **Open** to continue.

   ![Prompt to open file](./media/edge-learn-more-co-di/edge-clickonce-modal-1.png)

If the user tries to open the file, and the file was flagged as unsafe, a second popup is displayed.  This popup warns the user that the file was flagged as unsafe, and asks them if they’re sure they want to download the file.

The second popup only shows up if:

- the file is a ClickOnce or DirectInvoke file
- ClickOnce or DirectInvoke are enabled
- the file is flagged as unsafe

 ![Prompt to open unsafe file](./media/edge-learn-more-co-di/edge-clickonce-modal-2.png)

> [!NOTE]
> If ClickOnce or DirectInvoke are disabled, requested files are treated as regular downloads and if flagged as unsafe, will be marked as unsafe. This is consistent with the treatment of other unsafe downloads.

## ClickOnce and DirectInvoke policies

There are 2 group policies that you can use to enable or disable ClickOnce and DirectInvoke for enterprise users. These two policies are [ClickOnceEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#clickonceenabled) and [DirectInvokeEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#directinvokeenabled). These two policies are labeled in the Group Policy Editor as "Allow users to open files using the ClickOnce protocol" and "Allow users to open files using the DirectInvoke protocol" respectively.

## ClickOnce and DirectInvoke behavior

The following examples show file handling when ClickOnce and DirectInvoke are enabled or disabled.

### ClickOnce enabled

1. A user opens a link to a page that requests ClickOnce support and gets the prompt in the next screenshot.

   ![Prompt to open an unsafe file](./media/edge-learn-more-co-di/edge-clickonce-enabled-1.png)

2. After the user clicks **Open**, ClickOnce attempts to launch the application.

   ![ClickOnce tries to launch application](./media/edge-learn-more-co-di/edge-clickonce-enabled-launch-app.png)

3. After the user clicks **Open**, the browser shows a popup that asks the user if they're sure they want to install the application.

   ![Prompt to open the file](./media/edge-learn-more-co-di/edge-clickonce-enabled-2.png)

   > [!NOTE]
   > The interface, messaging, and options shown by the ClickOnce file handler will vary depending on the type and configuration of the file that's accessed.

### ClickOnce disabled

1. When a user opens a link to a page that requests ClickOnce support, they will see a message in the download tray that is similar to the one in the next screenshot.

   ![File download prompt](./media/edge-learn-more-co-di/edge-clickonce-disabled-1.png)

### DirectInvoke enabled

1. A user opens a link to a page that requests DirectInvoke support and gets the prompt in the next screenshot.

   ![Prompt to open file](./media/edge-learn-more-co-di/edge-directinvoke-open-link-1.png)

2. When the user clicks **Open**, the requested file handler is opened. In this example, Microsoft Word is used to open the document that's shown in the previous screenshot.

   > [!NOTE]
   > The interface, messaging, and options shown by the DirectInvoke file handler will vary depending on the type and configuration of the file that's accessed.

### DirectInvoke disabled

1. When a user opens a link to a page that requests DirectInvoke support, DirectInvoke behaves the same as when ClickOnce is disabled. They will see a message in the download tray that's similar to the one in the next screenshot.

   ![Prompt to open file](./media/edge-learn-more-co-di/edge-directinvoke-open-link-2.png)

## See also

- [ClickOnce security and deployment](https://go.microsoft.com/fwlink/?linkid=2099880)
- [DirectInvoke in Internet Explorer](https://go.microsoft.com/fwlink/?linkid=2099871)
