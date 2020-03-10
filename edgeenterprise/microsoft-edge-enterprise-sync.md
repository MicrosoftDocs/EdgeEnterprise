---
title: "Microsoft Edge Sync"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 02/14/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Sync"
---

# Microsoft Edge Sync

This article explains how to use Microsoft Edge to sync your favorites, passwords, and other browser data across all your signed-in devices.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Overview

Microsoft Edge sync enables users to access their browsing data across all their signed-in devices. The data supported by sync includes:

- Favorites
- Passwords
- Addresses and more (form-fill)
- Settings

Sync functionality is enabled via user consent and users can turn sync on or off for each of the data types listed above.

> [!NOTE]
> Additional device connectivity and configuration data (such as device name, make and model) is uploaded to support sync functionality.

## Prerequisites

Currently Microsoft Edge sync for Azure Active Directory (Azure AD) accounts is only available for the following subscriptions:

- Azure AD Premium (P1 and P2)
- Office 365 E3 and above
- Azure Information Protection (P1& P2)
- All EDU subscriptions (O365 A1 or above, M365 A1 or above, or AIP P1 or P2 for Students or Faculty)

> [!NOTE]
> Sync has a dependency on the protection service offered by Azure Information Protection (AIP) to protect sync data. This service is currently available to the preceding subscriptions. To see the full list of SKUs with AIP, see [Information Protection Pricing](https://azure.microsoft.com/pricing/details/information-protection/).

## Configuration options for Microsoft Edge sync

The following configuration options are available for enabling Microsoft Edge sync:

- Azure Information Protection (AIP)
- Azure AD Enterprise State Roaming (ESR)

If both AIP and ESR are disabled, users will see an error message indicating that sync is not available for their account.

### Azure Information Protection (AIP)

If the Azure Information Protection (AIP) service is enabled for a tenant, all users can sync Microsoft Edge data, regardless of licensing. Instructions on how to enable AIP can be found [here](https://docs.microsoft.com/azure/information-protection/activate-office365).

To restrict sync to certain set of users, the [AADRM onboarding control policy](https://docs.microsoft.com/powershell/module/aadrm/set-aadrmonboardingcontrolpolicy?view=azureipps) can be enabled for those users.

> [!CAUTION]
> This will also restrict access for other applications using Azure Information Protection, such as Microsoft Word or Microsoft Outlook.

### Azure AD Enterprise State Roaming (ESR)

If the Azure Active Directory [Enterprise State Roaming](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview) (ESR) feature is enabled for any user or tenant, they can use the Microsoft Edge sync feature regardless of the onboarding control policy setting.

## Microsoft Edge and Enterprise State Roaming

The new Microsoft Edge is a cross-platform application with an expanded scope for syncing user data across all their devices and is no longer a part of Azure AD Enterprise State Roaming. However, the new Microsoft Edge will fulfill the data protection promises of ESR, such as the ability to bring your own key. For more information, see [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md).

## Sync group policies

The following group policies impact Microsoft Edge sync:

- [SyncDisabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#syncdisabled): Disables sync completely.
- [SavingBrowserHistoryDisabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#savingbrowserhistorydisabled): Disables saving browsing history and sync. This also disables open-tabs sync.

## Frequently Asked Questions

### What happens with enterprise and educational customers who decide to stay with Microsoft Edge Legacy?

The current version of Microsoft Edge browser will continue to participate in the ESR offering.

### Where is sync data stored for Microsoft Edge?

Synced data for Azure AD accounts is stored in secure servers according to the tenant ID. For example, the data for a tenant that is registered in the United States is stored in servers geo-located for that region and leverages the same storage solution used by Office applications. While the synced data for Azure AD accounts is encrypted before leaving a user’s device, it is further encrypted when stored in the cloud.

### Will the new Chromium-based Microsoft Edge browser sync with the current in-market version of Microsoft Edge?

No, it won’t. We believe connecting these two ecosystems will lead to compromises in the reliability of sync in the new Microsoft Edge. We will ensure that existing data is migrated to the new Microsoft Edge. Users will also be able to import data from browser of their choice. This also means that new Microsoft Edge browser will not have a way to sync with IE.

### What about sync support for on-prem accounts?

Currently Microsoft Edge doesn't support sync for on-prem accounts. We will be adding this support in a future release.

### Is Microsoft Edge going to support sync for non-premium Azure AD accounts?

Yes, sync will be enabled for all paid Azure AD SKUs in future releases.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md)