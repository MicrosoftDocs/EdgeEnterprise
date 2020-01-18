---
title: "Access the old version of Microsoft Edge"
ms.author: jtkim
author: dan-wesley
manager: srugh
ms.date: 11/26/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "How to access the legacy version of Microsoft Edge."
---

# Access Microsoft Edge Legacy after installing the new version of Microsoft Edge

This article describes how to access Microsoft Edge Legacy (version 45 and earlier) after installing the new version of Microsoft Edge.

   > [!NOTE]
   > This article applies to the Microsoft Edge [Stable channel](microsoft-edge-channels.md).

The procedures in this article apply to systems that have been updated with the latest security updates. When the new version of Microsoft Edge is installed, the old version (Microsoft Edge Legacy) will be hidden. By default, all attempts to launch the old version will redirect the user to the newly installed version of Microsoft Edge. This article describes three different methods to enable Microsoft Edge Legacy to continue to be available.

## Before you begin

Before using the detailed instructions in this article, consider the following 2 steps to enable a side-by-side browser experience by preventing the Stable Channel of Microsoft Edge to be installed. These steps will let your users run Microsoft Edge Legacy and the next version of Microsoft Edge ([Beta channel](microsoft-edge-channels.md)) side-by-side.

1. Prevent the automatic install of the Stable Channel of the next version of Microsoft Edge by Windows Update. For more information, see [Windows Update: FAQ](https://support.microsoft.com/help/12373/windows-update-faq)
2. Install the [Beta channel](https://www.microsoftedgeinsider.com) of the new version of Microsoft Edge instead.

   > [!NOTE]
   > This side-by-side solution is less complex and requires less management than the detailed solution described in this article.
   > However, this does mean that you will be running the Beta Channel rather than the Stable Channel. 

## How to enable a side-by-side experience with both versions of Microsoft Edge

Installing the Stable channel of the next version of Microsoft Edge at the system-level will cause the current version (Microsoft Edge Legacy) to be hidden. If you want to let your users see both versions of Microsoft Edge side-by-side in Windows, you can enable this experience by setting the **Allow Microsoft Edge Side by Side browser experience** group policy to "Enabled".

This group policy is documented [here](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-update-policies#allowsxs).

### To enable the side-by-side browser experience policy:

1. Install the Policy Definitions from [Microsoft](https://www.microsoft.com/en-us/edge/business/download)
    - Set the build and platform as appropriate, and click to "Get Policy Files"
    - Extract the Zipped files
    - Copy msedge.admx and msedgeupdate.admx to the `c:\windows\PolicyDefinitions` directory
    - Copy msedge.adml and msedgeupdate.adml (from the appropriate language directory) to the `c:\windows\PolicyDefinitions\{APPROPIATE LANUGAGE}` directory
2. Open the Group Policy Editor (gpedit.msc)
3. Under **Computer Configuration**, go to *Administrative Templates>Microsoft Edge Update>Applications*.
   > [!NOTE]
   > If you do not see 'Microsoft Edge Update' available, verify that step 1 was completed correctly
4. Under **Applications**, select "Allow Microsoft Edge Side by Side browser experience" and then click Edit **policy setting**.
5. Select **Enabled** and then click **OK**.  
   > [!IMPORTANT]
   > Setting this policy will set the followoing Registry Key (as documented in the link above) to '00000001':
   > Key: `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate`
   > Value Name: `Allowsxs`
   > Value Type: 'REG_DWORD'
   
   > [!NOTE]
   > By default, this group policy is set to "Not configured", which results in Microsoft Edge Legacy being hidden when the new version of Microsoft Edge is installed.

For the best experience, the **Allow Microsoft Edge Side by Side browser experience** should be enabled before the new version of Microsoft Edge is deployed to your users' devices.

If the group policy is enabled after Microsoft Edge is deployed, there are the following side effects and required actions:

1. **Allow Microsoft Edge Side by Side browser experience** won't take effect until after the installer for the new version of Microsoft Edge is run again.

   > [!NOTE]
   > The installer can be run directly or automatically when the new version of Microsoft Edge updates.

2. Microsoft Edge Legacy will need to be re-pinned to Start or the Taskbar because the pin is migrated when the new version of Microsoft Edge is deployed.
3. Sites that were pinned to Start or the Taskbar for Microsoft Edge Legacy will be migrated to the new version of Microsoft Edge.

## How operating system (OS) changes are triggered

After the systems are fully updated and the Stable channel of the next version of Microsoft Edge is installed, the following registry key and value is set:

- Key: `Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\EdgeUpdate\ClientState\{56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}`
- Key value: `BrowserReplacement`

   > [!IMPORTANT]
   > This key is over-written every time the Microsoft Edge Stable channel is updated. As a best practice, we recommend that you do not delete this key to allow users to access both versions of Microsoft Edge.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Windows updates to support Microsoft Edge](microsoft-edge-sysupdate-windows-updates.md)
