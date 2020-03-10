---
title: "Microsoft Edge identity support and configuration"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 02/14/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge identity support and configuration"
---

# Microsoft Edge identity support and configuration

This article describes how Microsoft Edge uses identity to support features such as sync and single sign-on. Microsoft Edge supports signing in with Active Directory (AD), Azure Active Directory (Azure AD), and Microsoft accounts (MSA).

> [!NOTE]
> This applies  to Microsoft Edge version 77 or later.

## Overview

When users sign in, they automatically benefit from single sign-on (SSO) when they visit websites that support their logged in account. When signed in, users can choose to sync their browsing data between their devices. Signing in is also needed to use authenticated browser features such as the **Enterprise New tab page**, [Microsoft Search](https://docs.microsoft.com/microsoftsearch/) and [Microsoft Information Protection](https://www.microsoft.com/security/technology/information-protection).

## Authentication

To ensure that users are always authenticated and can benefit from authenticated features, they’re automatically signed into Microsoft Edge if they’re signed into Windows. Users can sign into Microsoft Edge with more than one account by adding a profile and then signing into it using a different account.

> [!NOTE]
> If users want to browse unauthenticated, they can add a profile or browse using the Guest profile.

## Authentication and features

The type of account used sign in determines which authentication and identity-based features are available and supported in Microsoft Edge. The following table summarizes the feature support for each type of account.

|                 | Azure AD Premium   | Azure AD Free      | On-premise AD | MSA           |
|-----------------|---------------|---------------|---------------|---------------|
| Sync            | Yes           | No            | No            | Yes           |
| SSO with Primary Refresh Token | Yes          |Yes          | No            | Yes          |
| Seamless SSO    | Yes           | Yes           | Yes           | N/A           |
| Windows Integrated Authentication | Yes          |Yes          |Yes          | N/A           |
| Enterprise New tab page | Requires O365 | Requires O365 | No            | N/A           |
| Microsoft Search | Requires O365 | Requires O365 | No           | N/A          |
| Microsoft Information Protection | Requires O365 E3 or E5 | Requires O365 E3 or E5 | Requires O365 E3 or E5 | N/A             |

### Single Sign-On

Microsoft Edge supports the following approaches to single sign-on.

#### Seamless SSO

Seamless Single Sign-On automatically signs users in when they are on corporate devices connected to a corporate network. When enabled, users don't need to type in their passwords to sign in to Azure AD, and usually, even type in their usernames. For more information, see [Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso).

#### SSO with Primary Refresh Token (PRT)

A Primary Refresh Token (PRT) is an Azure AD key that’s used for authentication on Windows 10, iOS, and Android devices. It enables single sign-on (SSO) across the applications used on those devices. For more information, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

#### Windows Integrated Authentication (WIA)

Windows Integrated Authentication (WIA) is enabled in Active Directory Federation Services (AD FS) for authentication requests within an organization's internal network for any application that uses a browser for its authentication. Microsoft Edge will only respond to WIA requests if the server is on the intranet. To configure which servers are enabled for integrated authentication, please see [the AuthServerAllowlist policy](https://docs.microsoft.com/deployedge/microsoft-edge-policies#authserverallowlist).

To use WIA with Microsoft Edge (version 77 and later) you have to configure the AD FS property **WiaSupportedUserAgents** and add support for the new Microsoft Edge user agent string. We use the "Edg" token to avoid compatibility issues that may be caused by using the string "Edge", which is used by the current version of Microsoft Edge based on EdgeHTML. The "Edg" token is also consistent with existing tokens used on iOS and Android. The following example of a UA string is for the latest Dev Channel build when this article was published:<br> `"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3951.0 Safari/537.36 Edg/80.0.334.2"`

For information about configuring WIA in AD FS, see [View WIASupportedUserAgent settings](https://docs.microsoft.com/windows-server/identity/ad-fs/operations/configure-ad-fs-browser-wia#view-wiasupporteduseragent-settings) and [Change WIASupportedUserAgent settings](https://docs.microsoft.com/windows-server/identity/ad-fs/operations/configure-ad-fs-browser-wia#change-wiasupporteduseragent-settings).

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)
- [Identity and access management](https://www.microsoft.com/security/technology/identity-access-management)
- [Identity platform](https://developer.microsoft.com/identity)
- [Four steps to a strong identity foundation with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/four-steps)
