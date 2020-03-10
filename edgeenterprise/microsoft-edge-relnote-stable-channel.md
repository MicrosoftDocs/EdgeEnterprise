---
title: "Microsoft Edge release notes for Stable Channel"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 03/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Stable Channel"
---

# Release notes for Microsoft Edge Stable Channel

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Stable Channel. All the security updates are listed [here](microsoft-edge-relnotes-security.md).

## Version 80.0.361.66: March 4

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#march-4-2020)

## Version 80.0.361.62: February 25

Security updates are listed [here](https://docs.microsoft.com/deployedge/microsoft-edge-relnotes-security#february-25-2020)

## Version 80.0.361.57: February 20

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#february-20-2020)

## Version 80.0.361.56: February 19

Fixed various bugs and performance issues.

## Version 80.0.361.54: February 14

### Resolved issues

- Fixed an issue where Password, Payment and Cookies fail to get imported in Microsoft Edge.

## Version 80.0.361.50: February 11

Fixed various bugs and performances fixes.

## Version 80.0.361.48: February 7

Security updates are listed [here](https://docs.microsoft.com/deployedge/microsoft-edge-relnotes-security#february-7-2020)

### Feature updates

- Added SmartScreen protection from downloading potentially unwanted apps. [Learn more](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus)
- Added support for Dolby Vision playback.
- Enabled users of Windows Mixed Reality to view 360° videos on VR headsets.
- Added an option to Reading View to increase text spacing.
- Added support for erasing link using the Surface Pen eraser.
- Added support for using the arrow keys and spacebar to draw on feedback screenshots in editor mode.
- Improved the reliability of screenshots so they stop appearing all black when submitting feedback.
- Added dark theme support to the local new tab page that is shown when the device isn't connected to the internet.
- Added the ability for websites installed as apps to be restored when a browser session is restored after update, crash, etc.
- Added dark theme support to PDF UI when the browser is managed by Group Policy.
- Updated Adobe Flash to version 32.0.0.321. [Learn more](https://helpx.adobe.com/flash-player/release-note/fp_32_air_32_release_notes.html)

### Policy updates

#### New policies

16 new policies were added. Download the updated Administrative Templates from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The following new policies were added.

- [AlternateErrorPagesEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#alternateerrorpagesenabled) - Suggest similar pages when a webpage can't be found.
- [DefaultInsecureContentSetting](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#defaultinsecurecontentsetting)  - Control use of insecure content exceptions.
- [DNSInterceptionChecksEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#dnsinterceptionchecksenabled) - DNS interception checks enabled.
- [HideFirstRunExperience](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#hidefirstrunexperience) - Hide the First-run experience and splash screen.
- [InsecureContentAllowedForUrls](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#insecurecontentallowedforurls) - Allow insecure content on specified sites.
- [InsecureContentBlockedForUrls](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#insecurecontentblockedforurls) - Block insecure content on specified sites.
- [LegacySameSiteCookieBehaviorEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#legacysamesitecookiebehaviorenabled) - Enable default legacy SameSite cookie behavior setting.
- [LegacySameSiteCookieBehaviorEnabledForDomainList](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) - Revert to legacy SameSite behavior for cookies on specified sites.
- [PaymentMethodQueryEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#paymentmethodqueryenabled) - Allow websites to query for available payment methods.
- [PersonalizationReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#personalizationreportingenabled) - Allow personalization of ads, search and news by sending browsing history to Microsoft.
- [PinningWizardAllowed](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#pinningwizardallowed) - Allow Pin to taskbar wizard.
- [SmartScreenPuaEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#smartscreenpuaenabled) - Configure Microsoft Defender SmartScreen to block potentially unwanted apps.
- [TotalMemoryLimitMb](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#totalmemorylimitmb) - Set limit on megabytes of memory a single Microsoft Edge instance can use.
- [WebAppInstallForceList](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webappinstallforcelist) - Configure list of force-installed Web Apps.
- [WebComponentsV0Enabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webcomponentsv0enabled) - Re-enable Web Components v0 API until M84.
- [WebRtcLocalIpsAllowedUrls](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webrtclocalipsallowedurls) - Manage exposure of local IP addresses by WebRTC.

#### Deprecated policies

The following policy was deprecated.

- [NewTabPageCompanyLogo](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#newtabpagecompanylogo) - Set new tab page company logo.

### Resolved issues

- Fixed an issue where audio is not working in Citrix environment.
- Fixed an issue where Microsoft Edge and legacy Microsoft Edge side by side experience results in broken legacy links and crashes.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
