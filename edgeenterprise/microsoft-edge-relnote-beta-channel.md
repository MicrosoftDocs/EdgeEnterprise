---
title: "Microsoft Edge release notes for Beta Channel"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 04/27/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Beta Channel"
---

# Release notes for Microsoft Edge Beta Channel

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Beta Channel.

> [!IMPORTANT]
> Please see this [update on Microsoft Edge channel releases](https://blogs.windows.com/msedgedev/2020/03/20/update-stable-channel-releases/).

## Version 83.0.478.18: April 27

Fixed various bugs and performance issues.

## Version 83.0.478.13: April 22

### Feature updates

- Microsoft Defender SmartScreen improvements: Made several improvements to the Microsoft Defender SmartScreen service, such as improved protection from malicious sites that redirect when loading, and top-level frame blocking, which completely replaces malicious sites with the Microsoft Defender SmartScreen safety page. The top-level frame blocking prevents audio and other media from the malicious site from playing which gives an easier and less confusing experience.

- In response to user feedback, users can now exempt certain cookies from automatically clearing when the browser closes. This option is helpful if there's a site that users don't want to be signed out of, but still want to have all the other cookies cleared when the browser closes. To use this feature, go to *edge://settings/clearBrowsingDataOnClose* and enable the "Cookies and other site data" toggle.

- Automatic Profile Switching is now available to help you get to your work content more easily across profiles. If you use multiple profiles at work, you can check it out by navigating to a site requiring authentication from your work or school account while on your personal profile. When we detect this, you will receive a prompt to switch to your work profile to access that site without having to authenticate to it. When you choose the work profile you want to switch to, the website will simply open in your work profile. This profile switching capability will help you keep your work and personal data separate and help you get to your work content more effortlessly. If you don't want the feature to prompt you to switch profiles, you can choose the don't ask me again option and it will get out of your way.

- Collections feature improvements:
  - You can use drag and drop to add an item to a collection without opening the collection. During the drag and drop you can also choose a location in the collection list where you want to put the item.
  - You can add multiple items to a collection instead of adding one item at a time. To add multiple items, select the items and then drag them to a collection. Or you can select the items, right-click and then pick the collection where you want the items.

- You can add all the tabs in an Edge window into a new collection without adding them individually. To do this, right-click on any tab and choose "Add all tabs to a new collection".

- Extension sync is now available. You can now sync your extensions across all your devices! Extensions from both the Microsoft and Chrome Stores will sync with Microsoft Edge. To use this feature: Click the ellipses (**…**) on the menu bar, select **Settings**. Under Your profile, click **Sync** to see the Sync options. Under **Profiles/Sync** use the toggle to enable Extensions. You can use the [SyncTypesListDisabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#synctypeslistdisabled) group policy to disable syncing of extensions.

- Improved the message on the Downloads management page for insecure downloads that have been blocked.

- Immersive Reader improvements:
  - Added support for Adverbs in the Parts of Speech experience we have in Immersive Reader. While reading an article within the Immersive Reader, open the Grammar Tools and switch on Adverbs within Parts of Speech to highlight all the adverbs on the page.
  - Added the ability to select any content on a webpage and open it in Immersive Reader. This ability enables users to use the Immersive Reader and all the Learning Tools, such as Line Focus and Read Aloud, across all websites.

- Link doctor provides host correction and a search query to the users when they mistype a URL. For example: <br>
A user mistypes "powerbi as "powerbbi".com. Link doctor will suggest "powerbi".com as a correction and create a link to search for "powerbbi" in case the user is looking for something different.

- Allow users to save their decision to launch an external protocol for a specific site. Users can configure the [ExternalProtocolDialogShowAlwaysOpenCheckbox]( https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#externalprotocoldialogshowalwaysopencheckbox) policy to enable or disable this feature.

- Users can set Microsoft Edge as their default browser directly from Microsoft Edge **Settings**. This makes it easier for users to change their default browser, within the context of the browser itself, instead of having to search through the operating system settings. To use this feature, go to *edge://settings/defaultBrowser* and click **Make default**.

- Several DevTools updates, including new remote debugging support, UI improvements, and more. For more details, see [What's New In DevTools (Microsoft Edge 83)](https://docs.microsoft.com/microsoft-edge/devtools-guide-chromium/whats-new/2020/03/devtools).

### Policy updates

#### New policies

15 new policies were added. Download the updated Administrative Templates from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The following new policies were added.

- [AllowSurfGame](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#allowsurfgame) - Allow surf game.
- [AllowTokenBindingForUrls](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#allowtokenbindingforurls) - Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with.
- [BingAdsSuppression](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#bingadssuppression) - Block all ads on Bing search results.
- [BuiltinCertificateVerifierEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#builtincertificateverifierenabled) - Determines whether the built-in certificate verifier will be used to verify server certificates.
- [ClearCachedImagesAndFilesOnExit](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#clearcachedimagesandfilesonexit) - Clear cached images and files when Microsoft Edge closes.
- [ConfigureShare](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#configureshare) - Configure the Share experience.
- [DeleteDataOnMigration](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#deletedataonmigration) - Delete old browser data on migration.
- [DnsOverHttpsMode](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#dnsoverhttpsmode) - Control the mode of DNS-over-HTTPS.
- [DnsOverHttpsTemplates](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#dnsoverhttpstemplates) - Specify URI template of desired DNS-over-HTTPS resolver.
- [FamilySafetySettingsEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#familysafetysettingsenabled) - Allow users to configure Family safety.
- [LocalProvidersEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#localprovidersenabled) - Allow suggestions from local providers.
- [ScrollToTextFragmentEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#scrolltotextfragmentenabled) - Enable scrolling to text specified in URL fragments.
- [ScreenCaptureAllowed](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#screencaptureallowed) - Allow or deny screen capture.
- [SyncTypesListDisabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#synctypeslistdisabled) - Configure the list of types that are excluded from synchronization.
- [NativeWindowOcclusionEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#nativewindowocclusionenabled) - Enable Hiding of Native Windows.

#### Deprecated policy

The following policy will continue to work in this release. It will become "obsolete" in a future release.

[EnableDomainActionsDownload](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#enabledomainactionsdownload) Enable Domain Actions Download from Microsoft

<!--  end 83 -->

## Version 81.0.416.60: April 20

Fixed various bugs and performance issues.

## Version 81.0.416.58: April 17

Security updates.

## Version 81.0.416.50: April 10

Fixed various bugs and performance issues.

## Version 81.0.416.45: April 3

Fixed various bugs and performance issues.

## Version 81.0.416.41: March 30

Fixed various bugs and performance issues.

## Version 81.0.416.34: March 17

Fixed various bugs and performance issues.

## Version 81.0.416.31: March 12

Fixed various bugs and performance issues.

## Version 81.0.416.28: March 9

Fixed various bugs and performance issues.

## Version 81.0.416.20: February 28

Fixed various bugs and performance issues.

## Version 81.0.416.12: February 20

### Feature updates

- Collections is now available. You can get started by clicking the Collections icon next to the address bar. This action opens the Collections pane where you can create, edit, and view Collections. We designed Collections based on what you do on the web. If you're a shopper, a traveler, a teacher, or a student, Collections can help. [Learn more](https://blogs.windows.com/msedgedev/2019/12/09/improvements-collections-sync-microsoft-edge/#LuDPRDUDCgdgdOVt.97).

- Allow the removal (Hide from toolbar) of the Collections button from the Microsoft Edge toolbar for consistency.

- On-prem Active Directory account auto sign in will only be targeted to organizations that turn it on.  If users were already signed in with an on-prem AD account, they will now be able to sign out of it. Now, users will only be automatically signed in with the primary account on their operating system if it is an MSA or an Azure AD account. Admins can enable auto sign in with an on-prem AD account using the ConfigureOnPremisesAccountAutoSignIn policy.

- Application Guard. Extensions support now available in the container.

- Added a message to inform users that Internet Explorer isn't installed when they navigate to a page that is configured to open in Internet Explorer mode.

- Updated the 3D View tool in Microsoft Edge DevTools with a new feature to help debug z-index stacking context. 3D View shows a representation of the DOM (Document Object Model) depth using color and stacking, and the z-Index view helps you isolate the different stacking contexts of your page. [Learn more](https://blogs.windows.com/msedgedev/2020/01/23/debug-z-index-3d-view-edge-devtools/).

- Localized the F12 Dev tools in 10 new languages, so they will match the language used in the rest of the browser. [Learn more](https://blogs.windows.com/msedgedev/2020/02/04/localizing-edge-devtools/).

- Added support for Dolby Vision playback. On Dolby Vision-enabled Windows 10 Build 17134 (April 2018 Update), websites can show Dolby vision content. See how to enable Dolby Vision content from [Netflix](https://help.netflix.com/en/node/42384).

- Microsoft Edge can now identify and remove duplicate favorites and merge folders with the same name. To access the tool, click the star on the browser's toolbar and select "Remove duplicate favorites".  You will be able to confirm changes and any updates to your favorites will be synced across devices.

- We heard from users it can be difficult to distinguish a normal browsing window in dark theme from an InPrivate window since both window frames are dark. The new solid InPrivate blue pill in the top right corner helps reassure users they are browsing InPrivate.

- Open external links in the correct browser profile. Select a default profile for links opened for external apps to open in from *edge://settings/multiProfileSettings*.

- Added a warning to alert users who sign into a browser profile with an account after being previously signed in with another account. This will help prevent unintentional data merging.

- If you have payment cards saved in your Microsoft account, you can use them in Microsoft Edge while filling out payment forms. The cards in your Microsoft account will sync across desktop devices and the full details will be shared with the website after two-factor authentication (CVC code and your Microsoft identity.) For further convenience, you can choose to securely save a copy of the card on the device during authentication.

- Line Focus is designed for users who like to focus on a limited part of the content as they read. It lets users keep the focus on 1, 3 or 5 lines at a time and dims out the rest of the page to let users read without distraction. Users can scroll using touch or arrow keys and the focus shifts accordingly.

- Microsoft Edge is now integrated with Windows Speller on Windows platforms 8.1 and above. This integration provides greater language support, with access to more language dictionaries and the ability to use Windows custom dictionaries. There is no further action needed from the users when a language has been added in the OS language settings and a language spellcheck toggle is enabled in Microsoft Edge settings.

- When PDF documents are opened using Microsoft Edge, users will now be able to create highlights, change color, and delete highlights. This helps in referencing important parts of the document later, and for collaboration.

- When loading long PDF documents that have been optimized for web, the pages being viewed by the user will be loaded faster, parallelly, while the rest of the document is loading.

- Now it's easier to start the Immersive Reader for a website by just pressing the F9 key.

- Now it's easier to start Read Aloud by using a keyboard shortcut (Ctrl + Shift + U).

### Policy updates

#### New policies

12 new policies were added. Download the updated Administrative Templates from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The following new policies were added.

- [AmbientAuthenticationInPrivateModesEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#ambientauthenticationinprivatemodesenabled) - Enable Ambient Authentication for InPrivate and Guest profiles. 
- [AudioSandboxEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#audiosandboxenabled) - Allow the audio sandbox to run.
- [ForceLegacyDefaultReferrerPolicy](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#forcelegacydefaultreferrerpolicy) - Use a default referrer policy of no-referrer-when-downgrade.
- [GloballyScopeHTTPAuthCacheEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#globallyscopehttpauthcacheenabled) - Enable globally scoped HTTP auth cache.
- [ImportExtensions](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importextensions) - Allow importing of extensions.
- [ImportCookies](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importcookies) - Allow importing of Cookies.
- [ImportShortcuts](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#importshortcuts) - Allow importing of shortcuts.
- [InternetExplorerIntegrationSiteRedirect](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#internetexplorerintegrationsiteredirect) - Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages.
- [OmniboxMSBProviderEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#omniboxmsbproviderenabled) - Enable Microsoft Search for Business provider in omnibox. 
- [StricterMixedContentTreatmentEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#strictermixedcontenttreatmentenabled) - Enable stricter treatment for mixed content.
- [TLS13HardeningForLocalAnchorsEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#tls13hardeningforlocalanchorsenabled) - Enable a TLS 1.3 security feature for local trust anchors.
- [ConfigureOnPremisesAccountAutoSignIn](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#configureonpremisesaccountautosignin) - Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account.

#### Deprecated policies

The following policies continue to work in this release. They will become "obsolete" in a future release.

- [WebComponentsV0Enabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webcomponentsv0enabled) - Re-enable Web Components v0 API until M84.
- [WebDriverOverridesIncompatiblePolicies](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#webdriveroverridesincompatiblepolicies) - Allow WebDriver to Override Incompatible.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
