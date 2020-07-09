---
title: "Microsoft Edge rollback for enterprises"
ms.author: v-danwes
author: dan-wesley
manager: srugh
ms.date: 07/08/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "How to rollback Microsoft Edge to a previous version"
---

# How to roll back Microsoft Edge to a previous version

This article describes how to roll back to a previous version of Microsoft Edge using the rollback feature.

>[!NOTE]
>This article applies to Microsoft Edge version 86 or later.

## Introduction to rollback

Rollback lets you replace your Microsoft Edge browser version with an earlier version. This feature is designed to be a safety net for enterprises deploying Microsoft Edge. It provides a way to troubleshoot issues with Microsoft Edge. The benefits of rollback are the ability to revert to previous browser version easily and quickly. Rollback reduces the potential impact that a Microsoft Edge issue has on business operations.

## Before you begin

It's important to understand how the rollback feature is installed in a Microsoft Edge environment. You can deploy rollback using two different methods: manually with an MSI or by using Microsoft Edge update and Group Policy. We also  encourage using a selection of Group Policies for a smoother deployment.

### Recommendations

The rollback feature is meant to be a temporary fix for issues you might find in a Microsoft Edge browser update. We recommend that users install the latest version of the Microsoft Edge browser to use the protection provided by the latest security updates. Rollback to an earlier version risks exposure to known security issues.

Before temporarily rolling back your browser version, we also highly recommend that you enable Sync for all the users in your organization. If you don't turn on Sync, there's a risk of permanent browsing data loss. For more information about Sync, see [Microsoft Edge Sync](microsoft-edge-enterprise-sync.md).

> [!CAUTION]
> Only use rollback when necessary, there's always the risk of data loss.

## Enable rollback manually with an MSI

Use the following steps to roll back manually with an MSI.

1. Disable Microsoft Edge Updates.

   > [!NOTE]
   > We recommend that you install the most current Administrative templates. For more information, see [Download and install the Microsoft Edge administrative template](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge#1-download-and-install-the-microsoft-edge-administrative-template).

   - Open the local Group Policy Editor and go to *Computer Configuration>Administrative Templates>Microsoft Edge Update>Applications>Microsoft Edge>*.
   - Select **Update policy override** and then select **Enabled**.
   - Under **Options**, pick **Update disabled** from the Policy dropdown list.

2. Get the MSI.

   - Download the MSI for the version you want to roll back to [from here](https://www.microsoft.com/edge/business/download).
   - Save the MSI to your desktop.

3. Run the rollback command.

   - Open the Windows command prompt with **Run as administrator**.
   - Type the following command, where: *C:\Users\username\Desktop\test* is the path to the MSI you downloaded, and FileName is the name of the .msi file:<br>
 `C:\Users\username\Desktop\test>msiexec /I FileName.msi ALLOWDOWNGRADE=1`
   - Close and re-open Microsoft Edge to verify that the rollback worked. Under **Settings and more** (ALT + F) go to **Settings** and select **About Microsoft Edge**.

## Enable rollback with Microsoft Edge update and Group Policy

Use the following steps to enable rollback with Microsoft Edge update and Group Policy.

1. Open the local Group Policy Editor and go to *Computer Configuration>Administrative Templates>Microsoft Edge Update>Applications>Microsoft Edge>*.
2. Select **Rollback to target version** and then select **Enabled**.
3. Select **Target version override** and pick the browser version you want to roll back to.
4. Select **Update policy override** and then select **Enabled**. Under **Options**, pick one of the following options from the Policy dropdown list (except for **Update disabled**):

   - Always allow updates
   - Automatic silent updates only
   - Manual updates only  

5. Rollback will happen the next time Microsoft Edge Update checks for an update.

   > [!NOTE]
   > If you want rollback to happen right away you have to change the Microsoft Edge Update polling interval or enable rollback using an MSI.

### Common rollback errors

The following errors will prevent rollback:

- Input is an unsupported target version
- Input is a non-existent target version
- Input is incorrectly formatted

### Recommended Group Policies

The following group policies and settings are highly recommended for using rollback.

#### Sync Group Policies

- ForceSync. Set ForceSync to enabled. This policy will force enable Sync on all Azure Active Directory (Azure AD) users. This policy is only effective for Microsoft Edge versions 86 and later.
- The *Configure the list of the types that are excluded from synchronization policy* allows admins to control what data can be synced by users.

#### Browser restart Group Policies

We recommend forcing a restart on users after rollback is enabled.

- Enable *Notify a user that a browser restart is recommended or required for pending updates*. Under Options, select **Required**.
- Enable *Set the time period for update notifications* and then set the desired time in milliseconds.

## Frequently asked questions

### Manual MSI rollback


### Microsoft Edge Update and Group Policy rollback



## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
