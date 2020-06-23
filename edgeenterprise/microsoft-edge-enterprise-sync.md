---
title: "Microsoft Edge Enterprise Sync"
ms.author: scottbo
author: dan-wesley
manager: silvanam
ms.date: 06/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Enterprise Sync"
---

# Microsoft Edge Enterprise Sync

This article explains how to use Microsoft Edge to sync your favorites, passwords, and other browser data across all your signed-in devices.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Overview

Microsoft Edge sync enables users to access their browsing data across all their signed-in devices. The data supported by sync includes:

- Favorites
- Passwords
- Addresses and more (form-fill)
- Collections
- Settings

Sync functionality is enabled via user consent and users can turn sync on or off for each of the data types listed above.

> [!NOTE]
> Additional device connectivity and configuration data (such as device name, make and model) is uploaded to support sync functionality.

## Prerequisites

Currently Microsoft Edge sync for Azure Active Directory (Azure AD) accounts is available for the following subscriptions:

- Azure AD Premium (P1 and P2)
- M365 Business Premium
- Office 365 E3 and above
- Azure Information Protection (AIP) (P1& P2)
- All EDU subscriptions (O365 A1 or above, M365 A1 or above, or Azure Information Protection P1 or P2 for Students or Faculty)

> [!NOTE]
> Sync has a dependency on the protection service offered by Azure Information Protection (AIP) to protect sync data. This service is currently available to the preceding subscriptions. To see the full list of SKUs with AIP, see [Information Protection Pricing](https://azure.microsoft.com/pricing/details/information-protection/).

## Configuration options for Microsoft Edge sync

The following configuration options are available for enabling Microsoft Edge sync:

- Azure Information Protection (AIP)
- Azure AD Enterprise State Roaming (ESR)

If both AIP and ESR are disabled, users will see an error message indicating that sync is not available for their account.

### Azure Information Protection (AIP)

If the Azure Information Protection (AIP) service is enabled for a tenant, all users can sync Microsoft Edge data, regardless of licensing. Instructions on how to enable AIP can be found [here](https://docs.microsoft.com/azure/information-protection/activate-office365).

To restrict sync to certain set of users, you can enable the [AADRM onboarding control policy](https://docs.microsoft.com/powershell/module/aadrm/set-aadrmonboardingcontrolpolicy?view=azureipps) for those users. If sync is still not available after ensuring that all necessary users are onboarded, ensure that the IPCv3Service is enabled using the [Get-AIPServiceIPCv3](https://docs.microsoft.com/powershell/module/aipservice/Get-AipServiceIPCv3?view=azureipps) PowerShell cmdlet.

> [!CAUTION]
> Activating Azure Information Protection will also restrict access for other applications using AIP, such as Microsoft Word or Microsoft Outlook.

### Azure AD Enterprise State Roaming (ESR)

If the Azure Active Directory [Enterprise State Roaming](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview) (ESR) feature is enabled for any user or tenant, they can use the Microsoft Edge sync feature regardless of the onboarding control policy setting.

## Microsoft Edge and Enterprise State Roaming

The new Microsoft Edge is a cross-platform application with an expanded scope for syncing user data across all their devices and is no longer a part of Azure AD Enterprise State Roaming. However, the new Microsoft Edge will fulfill the data protection promises of ESR, such as the ability to bring your own key. For more information, see [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md).

## Sync group policies

The following group policies impact Microsoft Edge sync:

- [SyncDisabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#syncdisabled): Disables sync completely.
- [SavingBrowserHistoryDisabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#savingbrowserhistorydisabled): Disables saving browsing history and sync. This policy also disables open-tabs sync.
- [SyncTypesListDisabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#synctypeslistdisabled): Configure the list of types that are excluded from synchronization.

## Frequently Asked Questions

### SECURITY and SERVER/DATA COMPLIANCE

#### Is the synced data encrypted? 

The data is encrypted in transport using TLS 1.2 or greater, and additionally at rest in Microsoft's service using AES256.

#### Where is Microsoft Edge sync data stored?

Synced data for Azure AD accounts is stored in secure servers according to the tenant ID. For example, the data for a tenant that is registered in the United States is stored in servers geo-located for that region and uses the same storage solution as Office applications.

#### Does the data ever leave Microsoft's cloud, aside from syncing to Microsoft Edge?

No.

#### Can tenant admins bring their own key?

Yes, through [Azure Information Protection](https://azure.microsoft.com/services/information-protection/).

#### What terms of service does enterprise sync fall under?

The terms of service are the same terms as your Azure AD subscription. All the Azure AD terms of service ultimately fall under Microsoft's [Online Service Terms](https://www.microsoft.com/licensing/product-licensing/products).

#### Does Microsoft Edge support Government Community Cloud (GCC) High compliance?

Not today. GCC High is Tier D, while Microsoft Edge supports up to Tier C.

### APPLYING SYNC

#### What happens with enterprise and educational customers who decide to stay with Microsoft Edge Legacy?

The current version of Microsoft Edge browser will continue to participate in the ESR offering.

#### Why do I need a premium Azure AD subscription to sync?

Enterprise sync depends on Azure Information Protection, which is not available in all Azure AD tiers.

#### Is Microsoft Edge sync based on Enterprise State Roaming?

No. ESR can be used to enable sync, but Microsoft Edge sync is not a part of ESR. For more information, see [Microsoft Edge Sync](microsoft-edge-enterprise-sync.md) and [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md).

#### Will Microsoft Edge ever support syncing between Microsoft Edge and IE?

There are no plans to support this syncing. If you still need IE in your environment to support legacy apps, consider our [new IE mode](https://docs.microsoft.com/deployedge/edge-ie-mode).

#### Will the new Microsoft Edge browser sync with Microsoft Edge Legacy?

No, it won't. We believe connecting these two ecosystems will lead to compromises in the reliability of sync in the new Microsoft Edge. We will ensure that existing data is migrated to the new Microsoft Edge. Users will also be able to import data from browser of their choice. This also means that new Microsoft Edge browser won't have a way to sync with IE.

### MANAGING SYNC

#### Is it possible to stop my users from syncing with a personal tenant?

Not directly, but you can determine which profiles can sign on to Microsoft Edge using the [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) policy.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md)
