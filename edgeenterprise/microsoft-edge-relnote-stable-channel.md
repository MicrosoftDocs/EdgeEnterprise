---
title: "Microsoft Edge release notes for Stable Channel"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 04/24/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Stable Channel"
---

# Release notes for Microsoft Edge Stable Channel

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Stable Channel. All the security updates are listed [here](microsoft-edge-relnotes-security.md).

> [!IMPORTANT]
> Please see this [update on Stable channel releases](https://blogs.windows.com/msedgedev/2020/03/20/update-stable-channel-releases/).

## Version 81.0.416.64: April 23

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#april-23-2020)

## Version 81.0.416.58: April 17

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#april-17-2020)

## Version 81.0.416.53: April 13

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#april-13-2020)

### Feature updates

- Added support for Windows Information Protection (WIP), which helps enterprises protect sensitive data from unauthorized disclosure. [Learn More](https://docs.microsoft.com/deployedge/microsoft-edge-security-windows-information-protection).

- Collections is now available. To get started, click the Collections icon next to the address bar. This action opens the Collections pane where you can create, edit, and view Collections. We designed Collections based on what you do on the web. If you're a shopper, a traveler, a teacher, or a student, Collections can help. [Learn more](https://blogs.windows.com/msedgedev/2019/12/09/improvements-collections-sync-microsoft-edge/#LuDPRDUDCgdgdOVt.97).

- Allow the removal (Hide from toolbar) of the Collections button from the Microsoft Edge toolbar for consistency.

- On-prem Active Directory account auto sign in will only be targeted to organizations that turn it on.  If users were already signed in with an on-prem AD account, they will be able to sign out of it. Users will only be automatically signed in with the primary account on their operating system if it's an MSA or an Azure AD account. Admins can enable auto sign in with an on-prem AD account using the ConfigureOnPremisesAccountAutoSignIn policy.

- Application Guard. Extensions support now available in the container.

- Added a message to inform users that Internet Explorer isn't installed when they navigate to a page that's configured to open in Internet Explorer mode.

- Updated the 3D View tool in Microsoft Edge DevTools with a new feature to help debug z-index stacking context. 3D View shows a representation of the DOM (Document Object Model) depth using color and stacking, and the z-Index view helps you isolate the different stacking contexts of your page. [Learn more](https://blogs.windows.com/msedgedev/2020/01/23/debug-z-index-3d-view-edge-devtools/).

- The F12 Dev tools are localized in 10 new languages, so they will match the language used in the rest of the browser. [Learn more](https://blogs.windows.com/msedgedev/2020/02/04/localizing-edge-devtools/).

- Added support for Dolby Vision playback. On Dolby Vision-enabled Windows 10 Build 17134 (April 2018 Update), websites can show Dolby vision content. See how to enable Dolby Vision content from [Netflix](https://help.netflix.com/en/node/42384).

- Microsoft Edge can now identify and remove duplicate favorites and merge folders with the same name. To access the tool, click the star on the browser's toolbar and select "Remove duplicate favorites".  You can that confirm changes and any updates to your favorites will be synced across devices.

- We heard from users it can be difficult to distinguish a normal browsing window in dark theme from an InPrivate window since both window frames are dark. The new solid InPrivate blue pill in the top right corner helps reassure users they are browsing InPrivate.

- Open external links in the correct browser profile. Select a default profile for links opened for external apps to open in from *edge://settings/multiProfileSettings*.

- Added a warning that alerts users who sign into a browser profile with an account after being previously signed in with another account. This warning will help prevent unintentional data merging.

- If you have payment cards saved in your Microsoft account, you can use them in Microsoft Edge while filling out payment forms. The cards in your Microsoft account will sync across desktop devices and the full details will be shared with the website after two-factor authentication (CVC code and your Microsoft identity.) For further convenience, you can choose to securely save a copy of the card on the device during authentication.

- Line Focus is designed for users who like to focus on a limited part of the content as they read. It lets users keep the focus on one, three, or five lines at a time and dims out the rest of the page to let users read without distraction. Users can scroll using touch or arrow keys and the focus shifts accordingly.

- Microsoft Edge is now integrated with Windows Speller on Windows platforms 8.1 and above. This integration provides greater language support, with access to more language dictionaries and the ability to use Windows custom dictionaries. There's no further action needed from the users when a language has been added in the OS language settings. Also, a language spellcheck toggle is enabled in Microsoft Edge settings.

- When PDF documents are opened using Microsoft Edge, users will now be able to create highlights, change color, and delete highlights. This feature helps in referencing important parts of the document later, and for collaboration.

- When loading long PDF documents that have been optimized for web, the pages being viewed by the user will be loaded faster, parallelly, while the rest of the document is loading.

- Now it's easier to start the Immersive Reader for a website by just pressing the F9 key.

- Now it's easier to start Read Aloud by using a keyboard shortcut (Ctrl + Shift + U).

- Added an MSI command line parameter that lets you suppress Desktop icon creation when you install Microsoft Edge. The following example shows how to use this new parameter: <br>
`MicrosoftEdgeEnterpriseX64.msi DONOTCREATEDESKTOPSHORTCUT=true`<br>
There will be a group policy to support this functionality in an upcoming release.

### Policy updates

#### New policies

11 new policies were added. Download the updated Administrative Templates from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The following new policies were added.

- [AmbientAuthenticationInPrivateModesEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#ambientauthenticationinprivatemodesenabled) - Enable Ambient Authentication for InPrivate and Guest profiles. 
- [AudioSandboxEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#audiosandboxenabled) - Allow the audio sandbox to run.
- [ForceLegacyDefaultReferrerPolicy](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#forcelegacydefaultreferrerpolicy) - Use a default referrer policy of no-referrer-when-downgrade.
- [GloballyScopeHTTPAuthCacheEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#globallyscopehttpauthcacheenabled) - Enable globally scoped HTTP auth cache.
- [ImportExtensions](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importextensions) - Allow importing of extensions.
- [ImportCookies](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importcookies) - Allow importing of Cookies.
- [ImportShortcuts](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importshortcuts) - Allow importing of shortcuts.
- [InternetExplorerIntegrationSiteRedirect](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#internetexplorerintegrationsiteredirect) - Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages.
- [StricterMixedContentTreatmentEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#strictermixedcontenttreatmentenabled) - Enable stricter treatment for mixed content.
- [TLS13HardeningForLocalAnchorsEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#tls13hardeningforlocalanchorsenabled) - Enable a TLS 1.3 security feature for local trust anchors.
- [ConfigureOnPremisesAccountAutoSignIn](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#configureonpremisesaccountautosignin) - Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account.

#### Policy name and caption changes

The policy `OmniboxMSBProviderEnabled` is changed to [AddressBarMicrosoftSearchInBingProviderEnabled](https://docs.microsoft.com//DeployEdge/microsoft-edge-policies#addressbarmicrosoftsearchinbingproviderenabled) - The caption for the policy is "Enable Microsoft Search in Bing suggestions in the address bar".

#### Deprecated policies

The following policies continue to work in this release. They will become "obsolete" in a future release.

- [WebComponentsV0Enabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webcomponentsv0enabled) - Re-enable Web Components v0 API until M84.
- [WebDriverOverridesIncompatiblePolicies](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webdriveroverridesincompatiblepolicies) - Allow WebDriver to Override Incompatible.

#### Resolved issues

- Fixed an issue where IE mode on Microsoft Edge caused an ongoing download dialog to show even after the file was downloaded.
- Fixed an issue where Microsoft Edge was dropping session cookies when a page already in IE mode triggered to open a new IE mode tab.

## Version 80.0.361.111: April 7

Fixed various bugs and performance issues.

## Version 80.0.361.109: April 1

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#april-1-2020)

## Version 80.0.361.69: March 19

Security updates are listed [here](https://docs.microsoft.com/DeployEdge/microsoft-edge-relnotes-security#march-19-2020)

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

- Fixed an issue where Password, Payment, and Cookies fail to get imported in Microsoft Edge.

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
- Added the ability for websites that are installed as apps to be restored when a browser session is restored after an update, crash, and so on.
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
- [PersonalizationReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#personalizationreportingenabled) - Allow personalization of ads, search, and news by sending browsing history to Microsoft.
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

- Fixed an issue where audio isn't working in Citrix environment.
- Fixed an issue where Microsoft Edge and legacy Microsoft Edge side-by-side experience results in broken legacy links and crashes.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
