---
title: "Microsoft Edge support for Microsoft Defender SmartScreen"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 04/13/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge support for Microsoft Defender SmartScreen"
---

# Microsoft Edge support for Microsoft Defender SmartScreen

This article describes the benefits of using Microsoft Defender SmartScreen, explains how it works, and describes how to configure this Microsoft Edge feature.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

Microsoft Defender SmartScreen is a service that Microsoft Edge uses to keep you safe while you browse the web. Microsoft Defender SmartScreen provides an early warning system against websites that might engage in phishing attacks or attempt to distribute malware through a focused attack.

> [!NOTE]
> Before Windows 10, version 1703, this feature was called the SmartScreen filter when used within the browser and Microsoft SmartScreen when used outside of the browser.

## The benefits of Microsoft Defender SmartScreen

Microsoft Defender SmartScreen provides several benefits, which are summarized in the following list. These benefits are described in detail in the [Microsoft Defender SmartScreen documentation](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-smartscreen/windows-defender-smartscreen-overview#benefits-of-windows-defender-smartscreen). The benefits are:

- Anti-phishing and anti-malware support
- Reputation-based URL and app protection
- Operating system integration
- Improved heuristics and diagnostic data
- Management through Group Policy and Microsoft Intune
- Blocking URLs associated with potentially unwanted applications

## Understand how Microsoft Defender SmartScreen works

A number of inputs contribute to Microsoft Defender SmartScreen warnings. We receive data from many sources, including user feedback, data providers, and intelligence models, and we use this data to help us identify potentially malicious content. Microsoft Defender SmartScreen also checks downloaded apps or app installers to see if they're malicious. In both scenarios, Microsoft Defender SmartScreen warns users appropriately about suspicious content.

### Site analysis

Microsoft Defender SmartScreen determines whether a site is potentially malicious by:

- Analyzing visited webpages looking for indications of suspicious behavior. If Microsoft Defender SmartScreen determines that a page is malicious, it will show a warning page to notify the user that that site is reported as unsafe.
- Checking the visited sites against a dynamic record of reported phishing sites. If it finds a match, Microsoft Defender SmartScreen shows a warning to let the user know that the site might contain phishing threats.

The next screenshot shows an example of a Microsoft Defender SmartScreen block page when a user tries to open a malicious website.

![Microsoft Defender SmartScreen block page for a link to external site](media/microsoft-edge-security-smartscreen/microsoft-edge-smartscreen-warning.png)

Users are giving the option of reporting a site as safe or unsafe from within the warning message. For more information, see [how to report a site](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-smartscreen/windows-defender-smartscreen-set-individual-device#how-users-can-report-websites-as-safe-or-unsafe).

### File analysis

Microsoft Defender SmartScreen determines whether a downloaded app or app installer is potentially malicious by:

- Checking downloaded files against reported malicious software sites and programs known to be unsafe sources. If it finds a match, Microsoft Defender SmartScreen shows a warning to let the user know that the site might be malicious.
- Checking downloaded files against a dynamic record of files that are well known and downloaded by many Windows users. If the file isn't on that list, Microsoft Defender SmartScreen shows a warning, advising caution.




> [!CAUTION]
> By default, Microsoft Defender SmartScreen lets users bypass warnings. Because this user interaction is potentially risky, we recommend that you review these [recommended group policy settings](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-smartscreen/windows-defender-smartscreen-available-settings#recommended-group-policy-and-mdm-settings-for-your-organization).

## Microsoft Defender SmartScreen and user privacy

Microsoft Defender SmartScreen keeps users safe while they browse the internet by using a reputation check system. Microsoft Edge passes relevant information about the URL or file to the Microsoft Defender SmartScreen service to start the reputation check. The check compares the website or file against dynamic lists of sites and files that are known to be dangerous. All requests to the Microsoft Defender SmartScreen service are made with TLS encryption. The service returns the results of the reputation check, which might lead to Microsoft Edge blocking the site or file. These results are stored locally on the device.

The Microsoft Defender SmartScreen service stores data about the reputation checks and builds a database of known malicious URLs and files. This data is stored on secure Microsoft servers and is only used for Microsoft security services. This data will never be used to identify or target users in any way. Clearing browsing cache clears all locally stored Microsoft Defender SmartScreen URL data. Clearing download history will remove any locally stored SmartScreen data about file downloads.

For more information about Microsoft Defender SmartScreen and privacy, read the [Microsoft Edge Privacy Whitepaper](https://docs.microsoft.com/microsoft-edge/privacy-whitepaper#smartscreen).

## Microsoft Defender SmartScreen setup for admins

Admins can set up Microsoft Defender SmartScreen using Group Policy, Microsoft Intune, and mobile device management (MDM) settings. Based on how you set up Microsoft Defender SmartScreen, you can show users a warning page and let them continue to the site, or block the site entirely.

### Microsoft Defender SmartScreen set up using Group Policy

For a complete list of SmartScreen policies, see
[Microsoft Defender SmartScreen settings](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#smartscreen-settings)

### Microsoft Defender SmartScreen set up using Microsoft Intune or MDM

For more information, see:

- [Windows Intune settings for Microsoft Defender SmartScreen](https://docs.microsoft.com/mem/intune/protect/endpoint-protection-windows-10#windows-defender-smartscreen-settings)
- [MDM policy settings](https://docs.microsoft.com/mem/intune/protect/endpoint-protection-windows-10#windows-defender-smartscreen-settings)

## Microsoft Defender SmartScreen setup for users

Microsoft Defender SmartScreen is turned on by default for Microsoft Edge. To turn off Microsoft Defender SmartScreen, go to *edge://settings/privacy > Services > Microsoft Defender SmartScreen*. This setting is the same for all profiles associated with the installation of Microsoft Edge on a device. This setting is not synced across devices. The setting applies to InPrivate browsing and Guest mode. If a device is managed with group policies set by an organization, this configuration will be reflected in *edge://settings/privacy*.

> [!NOTE]
> Users can set up Microsoft Defender SmartScreen for an individual device unless Group Policy or Microsoft Intune is configured to prevent it. For more information, see [set up and use Microsoft Defender SmartScreen on individual devices](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-smartscreen/windows-defender-smartscreen-set-individual-device).

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Threat protection](https://docs.microsoft.com/windows/security/threat-protection/index)