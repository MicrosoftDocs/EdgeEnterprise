---
title: "Microsoft Edge Update Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 10/30/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom:
description: "Documentation for all policies supported by the Microsoft Edge Updater"
---

# Microsoft Edge - Update policies

The latest version of Microsoft Edge includes the following policies that you can use to control how and when Microsoft Edge is updated.					  
For information about other policies available in Microsoft Edge, check out [Microsoft Edge browser policy reference](microsoft-edge-policies.md)
> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Available policies
These tables lists all of the update-related group policies available in this release of Microsoft Edge. Use the links in the table to get more details about specific policies.

|||
|-|-|
|[Applications](#applications)|[Preferences](#preferences)|
|[Proxy Server](#proxy-server)||

### [Applications](#applications-policies)
|Policy Name|Caption|
|-|-|
|[InstallDefault](#installdefault)|Allow installation default|
|[UpdateDefault](#updatedefault)|Update policy override default|
|[Install](#install)|Allow installation (per channel)|
|[Update](#update)|Update policy override (per channel)|
|[Allowsxs](#allowsxs)|Allow Microsoft Edge Side by Side browser experience|

### [Preferences](#preferences-policies)
|Policy Name|Caption|
|-|-|
|[AutoUpdateCheckPeriodMinutes](#autoupdatecheckperiodminutes)|Auto-update check period override|
|[UpdatesSuppressed](#updatessuppressed)|Time period in each day to suppress auto-update check|

### [Proxy Server](#proxy-server-policies)
|Policy Name|Caption|
|-|-|
|[ProxyMode](#proxymode)|Choose how to specify proxy server settings|
|[ProxyPacUrl](#proxypacurl)|URL to a proxy .pac file|
|[ProxyServer](#proxyserver)|Address or URL of proxy server|

## Applications policies

[Back to top](#microsoft-edge---update-policies)
### InstallDefault
#### Allow installation default
>Microsoft Edge Update 1.2.145.5 and later

#### Description
Lets you specify the default behavior for all channels where allowing or blocking Microsoft Edge browser installation by Microsoft Edge Update is concerned.

  Can be overridden for individual channels by specifying the ['Allow installation'](#install) policy for those specific channels. If you disable this policy, installation of Microsoft Edge through Microsoft Edge Update is blocked.

  Affects installation of Microsoft Edge software only when users are running Microsoft Edge Update and only when they haven't configured the ['Allow installation'](#install) policy.

  This policy doesn't prevent Microsoft Edge Update from running or prevent users from installing Microsoft Edge software by other methods.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: InstallDefault
- GP name: Allow installation default
- GP path: Administrative Templates/Microsoft Edge Update/Applications
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: InstallDefault
- Value Type: REG_DWORD
##### Example value:
```
0x00000001
```
[Back to top](#microsoft-edge---update-policies)


### UpdateDefault
#### Update policy override default
>Microsoft Edge Update 1.2.145.5 and later

#### Description
Lets you specify the default behavior for all channels concerning the way Microsoft Edge Update handles available updates for Microsoft Edge. Can be overridden for individual channels by specifying the ['Update policy override'](#update) policy for those specific channels.

  If you enable this policy, Microsoft Edge Update handles Microsoft Edge updates according to how you configure the following options:
   - Always allow updates: Updates are always applied when found, either by periodic update check or by a manual update check.
   - Automatic silent updates only: Updates are applied only when they're found by the periodic update check.
   - Manual updates only: Updates are applied only when the user runs a manual update check.
   - Updates disabled: Updates are never applied.

  If you select manual updates, make sure you periodically check for updates by using the app's manual update mechanism, if available. If you disable updates, periodically check for updates, and distribute them to users.

  If you don't enable and configure this policy, Microsoft Edge Update handles available updates as specified by the ['Update policy override'](#update) policy.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: UpdateDefault
- GP name: Update policy override default
- GP path: Administrative Templates/Microsoft Edge Update/Applications
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: UpdateDefault
- Value Type: REG_DWORD
##### Example value:
```
0x00000003
```
[Back to top](#microsoft-edge---update-policies)


### Install
#### Allow installation
>Microsoft Edge Update 1.2.145.5 and later

#### Description
Specifies whether a Microsoft Edge channel can be installed using Microsoft Edge Update.

  If you enable this policy for a channel, users can install that channel of Microsoft Edge through Microsoft Edge Update.

  If you disable this policy for a channel, users cannot install that channel of Microsoft Edge through Microsoft Edge Update.

  If you don't configure this policy for a channel, the ['Allow installation default'](#installdefault) policy configuration determines whether users can install that channel of Microsoft Edge through Microsoft Edge Update.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: Install
- GP name: Allow installation
- GP path: 
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Beta
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Canary
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Dev
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: 
  - (Stable): Install{56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}
  - (Beta): Install{2CD8A007-E189-409D-A2C8-9AF4EF3C72AA}
  - (Canary): Install{65C35B14-6C1D-4122-AC46-7148CC9D6497}
  - (Dev): Install{0D50BFEC-CD6A-4F9A-964C-C7416E3ACB10}
- Value Type: REG_DWORD
##### Example value:
```
0x00000001
```
[Back to top](#microsoft-edge---update-policies)


### Update
#### Update policy override
>Microsoft Edge Update 1.2.145.5 and later

#### Description
Specifies how Microsoft Edge Update handles available updates from Microsoft Edge.

  If you enable this policy, Microsoft Edge Update handles Microsoft Edge updates according to how you configure the following options:
   - Always allow updates: Updates are always applied when found, either by periodic update check or by a manual update check.
   - Automatic silent updates only: Updates are applied only when they're found by the periodic update check.
   - Manual updates only: Updates are applied only when the user runs a manual update check. (Not all apps provide an interface for this option.)
   - Updates disabled: Updates are never applied.

  If you select manual updates, make sure you periodically check for updates by using the app's manual update mechanism, if available. If you disable updates, periodically check for updates, and distribute them to users.

  If you don't enable and configure this policy, Microsoft Edge Update handles available updates as specified by the ['Update policy override default'](#updatedefault) policy.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: Update
- GP name: Update policy override
- GP path: 
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Beta
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Canary
  - Administrative Templates/Microsoft Edge Update/Applications/Microsoft Edge Dev
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: 
  - (Stable): Update{56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}
  - (Beta): Update{2CD8A007-E189-409D-A2C8-9AF4EF3C72AA}
  - (Canary): Update{65C35B14-6C1D-4122-AC46-7148CC9D6497}
  - (Dev): Update{0D50BFEC-CD6A-4F9A-964C-C7416E3ACB10}
- Value Type: REG_DWORD
##### Example value:
```
0x00000001
```
[Back to top](#microsoft-edge---update-policies)


### Allowsxs
#### Allow Microsoft Edge Side by Side browser experience
>Microsoft Edge Update 1.2.145.5 and later

#### Description
This policy lets a user run Microsoft Edge (Edge HTML) and Microsoft Edge (Chromium-based) side-by-side.

If this policy is set to “Not configured”, Microsoft Edge (Chromium-based) will replace Microsoft Edge (Edge HTML) after the Microsoft Edge (Chromium-based) stable channel and the November 2019 security updates are installed.  This is the same behavior as the “Disabled” setting.

The “Disabled” setting blocks a side-by-side experience and Microsoft Edge (Chromium-based) will replace Microsoft Edge (Edge HTML) after the Microsoft Edge (Chromium-based) stable channel and the November 2019 security updates are installed.  This is the same behavior as the “Not Configured” setting.

When this policy is “Enabled”, Microsoft Edge (Chromium-based) and Microsoft Edge (Edge HTML) can run side-by-side after Microsoft Edge (Chromium-based) is installed.

For this group policy to take affect, it must be configured before the automatic install of Microsoft Edge (Chromium-based) by Windows Update. Note: ​A user can block the automatic update of Microsoft Edge (Chromium-based) by using the Microsoft Edge (Chromium-based) Blocker Toolkit.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: Allowsxs
- GP name: Allow Microsoft Edge Side by Side browser experience
- GP path: Administrative Templates/Microsoft Edge Update/Applications
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: Allowsxs
- Value Type: REG_DWORD
##### Example value:
```
0x00000001
```
[Back to top](#microsoft-edge---update-policies)


## Preferences policies

[Back to top](#microsoft-edge---update-policies)
### AutoUpdateCheckPeriodMinutes
#### Auto-update check period override
>Microsoft Edge Update 1.2.145.5 and later

#### Description
If enabled, this policy lets you set a value for the minimum number of minutes between automatic update checks. Otherwise, by default, auto-update checks for updates every 10 hours.

  If you want to disable all auto-update checks, set the value to 0 (not recommended).
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: AutoUpdateCheckPeriodMinutes
- GP name: Auto-update check period override
- GP path: Administrative Templates/Microsoft Edge Update/Preferences
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: AutoUpdateCheckPeriodMinutes
- Value Type: REG_DWORD
##### Example value:
```
0x00000578
```
[Back to top](#microsoft-edge---update-policies)


### UpdatesSuppressed
#### Time period in each day to suppress auto-update check
>Microsoft Edge Update 1.3.33.5 and later

#### Description
If you enable this policy, update checks are suppressed each day starting at Hour:Minute for a period of Duration (in minutes). Duration isn't affected by daylight saving time. For example, if the start time is 22:00 and the duration is 480 minutes, updates will be suppressed for exactly 8 hours, regardless of whether daylight saving time starts or ends during this period.

  If you disable or don't configure this policy, update checks aren't suppressed during any specific period.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: UpdatesSuppressed
- GP name: Time period in each day to suppress auto-update check
  - Options { Hour, Minute, Duration }
- GP path: Administrative Templates/Microsoft Edge Update/Preferences
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: 
  - UpdatesSuppressedDurationMin
  - UpdatesSuppressedStartHour
  - UpdatesSuppressedStartMin
- Value Type: REG_DWORD
##### Example value:
```
duration   : 0x0000003c
start hour : 0x00000001
start min  : 0x00000002
```
[Back to top](#microsoft-edge---update-policies)


## Proxy Server policies
			  
		

[Back to top](#microsoft-edge---update-policies)
### ProxyMode
#### Choose how to specify proxy server settings
>Microsoft Edge Update 1.3.21.81 and later

#### Description
Allows you to specify the proxy server settings that are used by Microsoft Edge Update.

  If you enable this policy, you can choose between the following proxy server options:
   - If you choose to never use a proxy server and always connect directly, all other options are ignored.
   - If you choose to use system proxy settings or auto-detect the proxy server, all other options are ignored.
   - If you choose fixed server proxy mode, you can specify further options in ['Address or URL of proxy server'](#proxyserver).
   - If you choose to use a .pac proxy script, you must specify the URL for the script in ['URL to a proxy .pac file'](#proxypacurl).

  If you enable this policy, users in your organization can't change the proxy settings in Microsoft Edge Update.

  If you disable or don't configure this policy, no proxy server settings are configured, but users in your organization can choose their own proxy settings for Microsoft Edge Update.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: ProxyMode
- GP name: Choose how to specify proxy server settings
- GP path: Administrative Templates/Microsoft Edge Update/Proxy Server
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: ProxyMode
- Value Type: REG_SZ
##### Example value:
```
fixed_servers
```
[Back to top](#microsoft-edge---update-policies)


### ProxyPacUrl
#### URL to a proxy .pac file
>Microsoft Edge Update 1.3.21.81 and later

#### Description
Allows you to specify a URL for a proxy auto-config (PAC) file.

  If you enable this policy, you can specify a URL for a PAC file to automate how Microsoft Edge Update selects the appropriate proxy server for fetching a particular website.

  This policy is applied only if you have specified manual proxy settings in the ['Choose how to specify proxy server settings'](#proxymode) policy.

  Don't configure this policy if you have selected a proxy setting other than manual in the ['Choose how to specify proxy server settings'](#proxymode) policy.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: ProxyPacUrl
- GP name: URL to a proxy .pac file
- GP path: Administrative Templates/Microsoft Edge Update/Proxy Server
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: ProxyPacUrl
- Value Type: REG_SZ
##### Example value:
```
https://www.microsoft.com
```
[Back to top](#microsoft-edge---update-policies)


### ProxyServer
#### Address or URL of proxy server
>Microsoft Edge Update 1.3.21.81 and later

#### Description
Allows you to specify the URL of the proxy server for Microsoft Edge Update to use.

  If you enable this policy, you can set the proxy server URL used by Microsoft Edge Update in your organization.

  This policy is applied only if you have selected manual proxy settings in the ['Choose how to specify proxy server settings'](#proxymode) policy.

  Don't configure this policy if you have selected a proxy setting other than manual in the ['Choose how to specify proxy server settings'](#proxymode) policy.
#### Windows information and settings
##### Group Policy (ADMX) info
- GP unique name: ProxyServer
- GP name: Address or URL of proxy server
- GP path: Administrative Templates/Microsoft Edge Update/Proxy Server
- GP ADMX file name: edgeupdate.admx
##### Windows Registry Settings
- Path: HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\EdgeUpdate
- Value Name: ProxyServer
- Value Type: REG_SZ
##### Example value:
```
https://www.microsoft.com
```
[Back to top](#microsoft-edge---update-policies)

		   

## See also
  - [Configuring Microsoft Edge](configure-microsoft-edge.md)
  - [Download Microsoft Edge For Enterprise](https://aka.ms/EdgeEnterprise)
