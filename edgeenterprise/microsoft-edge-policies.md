---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 03/27/2020
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - Policies
The latest version of Microsoft Edge includes the following policies. You can use these policies to configure how Microsoft Edge runs in your organization.

For information about an additional set of policies used to control how and when Microsoft Edge is updated, check out [Microsoft Edge update policy reference](microsoft-edge-update-policies.md).

You can download the [Microsoft Security Compliance Toolkit](https://www.microsoft.com/download/details.aspx?id=55319) for the recommended security configuration baseline settings for Microsoft Edge. For more information see the [Microsoft Security Baselines Blog](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/bg-p/Microsoft-Security-Baselines).

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Available policies
These tables list all of the browser-related group policies available in this release of Microsoft Edge. Use the links in the table to get more details about specific policies.

|||
|-|-|
|[Cast](#cast)|[Content settings](#content-settings)|
|[Default search provider](#default-search-provider)|[Extensions](#extensions)|
|[HTTP authentication](#http-authentication)|[Native Messaging](#native-messaging)|
|[Password manager and protection](#password-manager-and-protection)|[Printing](#printing)|
|[Proxy server](#proxy-server)|[SmartScreen settings](#smartscreen-settings)|
|[Startup, home page and new tab page](#startup-home-page-and-new-tab-page)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|Policy Name|Caption|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Enable Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Show the cast icon in the toolbar|
### [*Content settings*](#content-settings-policies)
|Policy Name|Caption|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Automatically select client certificates for these sites|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Allow cookies on specific sites|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Block cookies on specific sites|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Limit cookies from specific websites to the current session|
|[DefaultCookiesSetting](#defaultcookiessetting)|Configure cookies|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Default geolocation setting|
|[DefaultImagesSetting](#defaultimagessetting)|Default images setting|
|[DefaultInsecureContentSetting](#defaultinsecurecontentsetting)|Control use of insecure content exceptions|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Default JavaScript setting|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Default notification setting|
|[DefaultPluginsSetting](#defaultpluginssetting)|Default Adobe Flash setting|
|[DefaultPopupsSetting](#defaultpopupssetting)|Default pop-up window setting|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Control use of the Web Bluetooth API|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Control use of the WebUSB API|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Allow images on these sites|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Block images on specific sites|
|[InsecureContentAllowedForUrls](#insecurecontentallowedforurls)|Allow insecure content on specified sites|
|[InsecureContentBlockedForUrls](#insecurecontentblockedforurls)|Block insecure content on specified sites|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Allow JavaScript on specific sites|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Block JavaScript on specific sites|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Enable default legacy SameSite cookie behavior setting|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Revert to legacy SameSite behavior for cookies on specified sites|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Allow notifications on specific sites|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Block notifications on specific sites|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Allow the Adobe Flash plug-in on specific sites|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Block the Adobe Flash plug-in on specific sites|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Allow pop-up windows on specific sites|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Block pop-up windows on specific sites|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Register protocol handlers|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Grant access to specific sites to connect to specific USB devices|
|[WebUsbAskForUrls](#webusbaskforurls)|Allow WebUSB on specific sites|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|Block WebUSB on specific sites|
### [*Default search provider*](#default-search-provider-policies)
|Policy Name|Caption|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Enable the default search provider|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Default search provider encodings|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Specifies the search-by-image feature for the default search provider|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Parameters for an image URL that uses POST|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Default search provider keyword|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Default search provider name|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|Default search provider search URL|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|Default search provider URL for suggestions|
### [*Extensions*](#extensions-policies)
|Policy Name|Caption|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Configure allowed extension types|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Allow specific extensions to be installed|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Control which extensions cannot be installed|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Control which extensions are installed silently|
|[ExtensionInstallSources](#extensioninstallsources)|Configure extension and user script install sources|
|[ExtensionSettings](#extensionsettings)|Configure extension management settings|
### [*HTTP authentication*](#http-authentication-policies)
|Policy Name|Caption|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Allow cross-origin HTTP Basic Auth prompts|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Specifies a list of servers that Microsoft Edge can delegate user credentials to|
|[AuthSchemes](#authschemes)|Supported authentication schemes|
|[AuthServerAllowlist](#authserverallowlist)|Configure list of allowed authentication servers|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Disable CNAME lookup when negotiating Kerberos authentication|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Include non-standard port in Kerberos SPN|
|[NtlmV2Enabled](#ntlmv2enabled)|Control whether NTLMv2 authentication is enabled|
### [*Native Messaging*](#native-messaging-policies)
|Policy Name|Caption|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Control which native messaging hosts users can use|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Configure native messaging block list|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Allow user-level native messaging hosts (installed without admin permissions)|
### [*Password manager and protection*](#password-manager-and-protection-policies)
|Policy Name|Caption|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Enable saving passwords to the password manager|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|Configure the change password URL|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Configure the list of enterprise login URLs where password protection service should capture fingerprint of password|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Configure password protection warning trigger|
### [*Printing*](#printing-policies)
|Policy Name|Caption|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Default printer selection rules|
|[PrintHeaderFooter](#printheaderfooter)|Print headers and footers|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Set the system default printer as the default printer|
|[PrintingEnabled](#printingenabled)|Enable printing|
|[UseSystemPrintDialog](#usesystemprintdialog)|Print using system print dialog|
### [*Proxy server*](#proxy-server-policies)
|Policy Name|Caption|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Configure proxy bypass rules|
|[ProxyMode](#proxymode)|Configure proxy server settings|
|[ProxyPacUrl](#proxypacurl)|Set the proxy .pac file URL|
|[ProxyServer](#proxyserver)|Configure address or URL of proxy server|
|[ProxySettings](#proxysettings)|Proxy settings|
### [*SmartScreen settings*](#smartscreen-settings-policies)
|Policy Name|Caption|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Prevent bypassing Microsoft Defender SmartScreen prompts for sites|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Configure the list of domains for which Microsoft Defender SmartScreen won't trigger warnings|
|[SmartScreenEnabled](#smartscreenenabled)|Configure Microsoft Defender SmartScreen|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Force Microsoft Defender SmartScreen checks on downloads from trusted sources|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
### [*Startup&comma; home page and new tab page*](#startup-home-page-and-new-tab-page-policies)
|Policy Name|Caption|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Set the new tab page as the home page|
|[HomepageLocation](#homepagelocation)|Configure the home page URL|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Set new tab page company logo %s(deprecated)|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Hide the default top sites from the new tab page|
|[NewTabPageLocation](#newtabpagelocation)|Configure the new tab page URL|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Set new tab page quick links|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configure the Microsoft Edge new tab page experience|
|[RestoreOnStartup](#restoreonstartup)|Action to take on startup|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Sites to open when the browser starts|
|[ShowHomeButton](#showhomebutton)|Show Home button on toolbar|
### [*Additional*](#additional-policies)
|Policy Name|Caption|
|-|-|
|[AddressBarMicrosoftSearchInBingProviderEnabled](#addressbarmicrosoftsearchinbingproviderenabled)|Enable Microsoft Search in Bing suggestions in the address bar|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Ads setting for sites with intrusive ads|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Enable deleting browser and download history|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Allow file selection dialogs|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Allows a page to show popups during its unloading|
|[AllowSurfGame](#allowsurfgame)|Allow surf game|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Allow pages to send synchronous XHR requests during page dismissal|
|[AllowTokenBindingForUrls](#allowtokenbindingforurls)|Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with.|
|[AllowTrackingForUrls](#allowtrackingforurls)|Configure tracking prevention exceptions for specific sites|
|[AlternateErrorPagesEnabled](#alternateerrorpagesenabled)|Suggest similar pages when a webpage can’t be found|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Always open PDF files externally|
|[AmbientAuthenticationInPrivateModesEnabled](#ambientauthenticationinprivatemodesenabled)|Enable Ambient Authentication for InPrivate and Guest profiles|
|[ApplicationLocaleValue](#applicationlocalevalue)|Set application locale|
|[AudioCaptureAllowed](#audiocaptureallowed)|Allow or block audio capture|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Sites that can access audio capture devices without requesting permission|
|[AudioSandboxEnabled](#audiosandboxenabled)|Allow the audio sandbox to run|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Automatically import another browser's data and settings at first run|
|[AutofillAddressEnabled](#autofilladdressenabled)|Enable AutoFill for addresses|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Enable AutoFill for credit cards|
|[AutoplayAllowed](#autoplayallowed)|Allow media autoplay for websites|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Continue running background apps after Microsoft Edge closes|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Enables background updates to the list of available templates for Collections and other features that use templates|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Block third party cookies|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Enable profile creation from the Identity flyout menu or the Settings page|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Enable guest mode|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Allow queries to a Browser Network Time service|
|[BrowserSignin](#browsersignin)|Browser sign-in settings|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Use built-in DNS client|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Disable Certificate Transparency enforcement for a list of legacy certificate authorities|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Disable Certificate Transparency enforcement for specific URLs|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Clear browsing data when Microsoft Edge closes|
|[ClearCachedImagesAndFilesOnExit](#clearcachedimagesandfilesonexit)|Clear cached images and files when Microsoft Edge closes|
|[ClickOnceEnabled](#clickonceenabled)|Allow users to open files using the ClickOnce protocol|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Enable security warnings for command-line flags|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Enable component updates in Microsoft Edge|
|[ConfigureDoNotTrack](#configuredonottrack)|Configure Do Not Track|
|[ConfigureOnPremisesAccountAutoSignIn](#configureonpremisesaccountautosignin)|Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Configure Online Text To Speech|
|[ConfigureShare](#configureshare)|Configure the Share experience|
|[CustomHelpLink](#customhelplink)|Specify custom help link|
|[DNSInterceptionChecksEnabled](#dnsinterceptionchecksenabled)|DNS interception checks enabled|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Set Microsoft Edge as default browser|
|[DeleteDataOnMigration](#deletedataonmigration)|Delete old browser data on migration|
|[DeveloperToolsAvailability](#developertoolsavailability)|Control where developer tools can be used|
|[DirectInvokeEnabled](#directinvokeenabled)|Allow users to open files using the DirectInvoke protocol|
|[Disable3DAPIs](#disable3dapis)|Disable support for 3D graphics APIs|
|[DisableScreenshots](#disablescreenshots)|Disable taking screenshots|
|[DiskCacheDir](#diskcachedir)|Set disk cache directory|
|[DiskCacheSize](#diskcachesize)|Set disk cache size, in bytes|
|[DnsOverHttpsTemplates](#dnsoverhttpstemplates)|Specify URI template of desired DNS-over-HTTPS resolver|
|[DownloadDirectory](#downloaddirectory)|Set download directory|
|[DownloadRestrictions](#downloadrestrictions)|Allow download restrictions|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Enable the Collections feature|
|[EditFavoritesEnabled](#editfavoritesenabled)|Allows users to edit favorites|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Re-enable deprecated web platform features for a limited time|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Enable Domain Actions Download from Microsoft %s(deprecated)|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Enable online OCSP/CRL checks|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Allow managed extensions to use the Enterprise Hardware Platform API|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Control communication with the Experimentation and Configuration Service|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Show an "Always open" checkbox in external protocol dialog|
|[FamilySafetySettingsEnabled](#familysafetysettingsenabled)|Allow users to configure Family safety|
|[FavoritesBarEnabled](#favoritesbarenabled)|Enable favorites bar|
|[ForceBingSafeSearch](#forcebingsafesearch)|Enforce Bing SafeSearch|
|[ForceCertificatePromptsOnMultipleMatches](#forcecertificatepromptsonmultiplematches)|Configure whether Microsoft Edge should automatically select a certificate when there are multiple certificate matches for a site configured with "AutoSelectCertificateForUrls"|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Enable use of ephemeral profiles|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Enforce Google SafeSearch|
|[ForceLegacyDefaultReferrerPolicy](#forcelegacydefaultreferrerpolicy)|Use a default referrer policy of no-referrer-when-downgrade. %s(deprecated)|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Force networking code to run in the browser process|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Force minimum YouTube Restricted Mode|
|[FullscreenAllowed](#fullscreenallowed)|Allow full screen mode|
|[GloballyScopeHTTPAuthCacheEnabled](#globallyscopehttpauthcacheenabled)|Enable globally scoped HTTP auth cache|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|Force direct intranet site navigation instead of searching on single word entries in the Address Bar|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Configure the list of names that will bypass the HSTS policy check|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Use hardware acceleration when available|
|[HideFirstRunExperience](#hidefirstrunexperience)|Hide the First-run experience and splash screen|
|[ImportAutofillFormData](#importautofillformdata)|Allow importing of autofill form data|
|[ImportBrowserSettings](#importbrowsersettings)|Allow importing of browser settings|
|[ImportCookies](#importcookies)|Allow importing of Cookies|
|[ImportExtensions](#importextensions)|Allow importing of extensions|
|[ImportFavorites](#importfavorites)|Allow importing of favorites|
|[ImportHistory](#importhistory)|Allow importing of browsing history|
|[ImportHomepage](#importhomepage)|Allow importing of home page settings|
|[ImportOpenTabs](#importopentabs)|Allow importing of open tabs|
|[ImportPaymentInfo](#importpaymentinfo)|Allow importing of payment info|
|[ImportSavedPasswords](#importsavedpasswords)|Allow importing of saved passwords|
|[ImportSearchEngine](#importsearchengine)|Allow importing of search engine settings|
|[ImportShortcuts](#importshortcuts)|Allow importing of shortcuts|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Configure InPrivate mode availability|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Configure Internet Explorer integration|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Configure the Enterprise Mode Site List|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages|
|[IsolateOrigins](#isolateorigins)|Enable site isolation for specific origins|
|[ManagedFavorites](#managedfavorites)|Configure favorites|
|[ManagedSearchEngines](#managedsearchengines)|Manage Search Engines|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Maximum number of concurrent connections to the proxy server|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Allow Google Cast to connect to Cast devices on all IP addresses|
|[MetricsReportingEnabled](#metricsreportingenabled)|Enable usage and crash-related data reporting|
|[NativeWindowOcclusionEnabled](#nativewindowocclusionenabled)|Enable Hiding of Native Windows|
|[NetworkPredictionOptions](#networkpredictionoptions)|Enable network prediction|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Configure whether a user always has a default profile automatically signed in with their work or school account|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Control where security restrictions on insecure origins apply|
|[PaymentMethodQueryEnabled](#paymentmethodqueryenabled)|Allow websites to query for available payment methods|
|[PersonalizationReportingEnabled](#personalizationreportingenabled)|Allow personalization of ads, search and news by sending browsing history to Microsoft|
|[PinningWizardAllowed](#pinningwizardallowed)|Allow Pin to taskbar wizard|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Enable Proactive Authentication|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Enable full-tab promotional content|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Ask where to save downloaded files|
|[QuicAllowed](#quicallowed)|Allow QUIC protocol|
|[RelaunchNotification](#relaunchnotification)|Notify a user that a browser restart is recommended or required for pending updates|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Set the time period for update notifications|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Enable renderer code integrity|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Specify if online OCSP/CRL checks are required for local trust anchors|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Enable resolution of navigation errors using a web service|
|[RestrictSigninToPattern](#restrictsignintopattern)|Restrict which accounts can be used as Microsoft Edge primary accounts|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Extend Adobe Flash content setting to all content|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Allow users to proceed from the HTTPS warning page|
|[SSLVersionMin](#sslversionmin)|Minimum TLS version enabled|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Disable saving browser history|
|[ScreenCaptureAllowed](#screencaptureallowed)|Allow or deny screen capture|
|[ScrollToTextFragmentEnabled](#scrolltotextfragmentenabled)|Enable scrolling to text specified in URL fragments|
|[SearchSuggestEnabled](#searchsuggestenabled)|Enable search suggestions|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Websites or domains that don't need permission to use direct Security Key attestation|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Send all intranet sites to Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Send site information to improve Microsoft services|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Show Microsoft Office shortcut in favorites bar|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Enable Signed HTTP Exchange (SXG) support|
|[SitePerProcess](#siteperprocess)|Enable site isolation for every site|
|[SpellcheckEnabled](#spellcheckenabled)|Enable spellcheck|
|[SpellcheckLanguage](#spellchecklanguage)|Enable specific spellcheck languages|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Force disable spellcheck languages|
|[StricterMixedContentTreatmentEnabled](#strictermixedcontenttreatmentenabled)|Enable stricter treatment for mixed content|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Suppress the unsupported OS warning|
|[SyncDisabled](#syncdisabled)|Disable synchronization of data using Microsoft sync services|
|[TLS13HardeningForLocalAnchorsEnabled](#tls13hardeningforlocalanchorsenabled)|Enable a TLS 1.3 security feature for local trust anchors.|
|[TabFreezingEnabled](#tabfreezingenabled)|Allow freezing of background tabs|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Enable ending processes in the Browser task manager|
|[TotalMemoryLimitMb](#totalmemorylimitmb)|Set limit on megabytes of memory a single Microsoft Edge instance can use.|
|[TrackingPrevention](#trackingprevention)|Block tracking of users' web-browsing activity|
|[TranslateEnabled](#translateenabled)|Enable Translate|
|[URLAllowlist](#urlallowlist)|Define a list of allowed URLs|
|[URLBlocklist](#urlblocklist)|Block access to a list of URLs|
|[UserDataDir](#userdatadir)|Set the user data directory|
|[UserFeedbackAllowed](#userfeedbackallowed)|Allow user feedback|
|[VideoCaptureAllowed](#videocaptureallowed)|Allow or block video capture|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Sites that can access video capture devices without requesting permission|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|Set WPAD optimization|
|[WebAppInstallForceList](#webappinstallforcelist)|Configure list of force-installed Web Apps|
|[WebComponentsV0Enabled](#webcomponentsv0enabled)|Re-enable Web Components v0 API until M84. %s(deprecated)|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Allow WebDriver to Override Incompatible Policies %s(deprecated)|
|[WebRtcLocalIpsAllowedUrls](#webrtclocalipsallowedurls)|Manage exposure of local IP addressess by WebRTC|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Restrict exposure of local IP address by WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Restrict the range of local UDP ports used by WebRTC|




  ## Cast policies

  [Back to top](#microsoft-edge---policies)

  ### EnableMediaRouter
  #### Enable Google Cast
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enable this policy to enable Google Cast. Users will be able to launch it from the app menu, page context menus, media controls on Cast-enabled websites, and (if shown) the Cast toolbar icon.

Disable this policy to disable Google Cast.

By default, Google Cast is enabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnableMediaRouter
  - GP name: Enable Google Cast
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Cast
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EnableMediaRouter
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: EnableMediaRouter
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ShowCastIconInToolbar
  #### Show the cast icon in the toolbar
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the [EnableMediaRouter](#enablemediarouter) policy to false, then this policy is ignored, and the toolbar icon isn't shown.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ShowCastIconInToolbar
  - GP name: Show the cast icon in the toolbar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Cast
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ShowCastIconInToolbar
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ShowCastIconInToolbar
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Content settings policies

  [Back to top](#microsoft-edge---policies)

  ### AutoSelectCertificateForUrls
  #### Automatically select client certificates for these sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. Each dictionary must have the form { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser will automatically select. Independent of the filter, only certificates will be selected that match the server's certificate request. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates are selected that are issued by a certificate with the CommonName $ISSUER_CN. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must satisfy both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization which matches the specified value to be selected. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value to be selected. If $FILTER is the empty dictionary {}, the selection of client certificates is not additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AutoSelectCertificateForUrls
  - GP name: Automatically select client certificates for these sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\1 = {"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}

```


  #### Mac information and settings
  - Preference Key Name: AutoSelectCertificateForUrls
  - Example value:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CookiesAllowedForUrls
  #### Allow cookies on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesBlockedForUrls](#cookiesblockedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CookiesAllowedForUrls
  - GP name: Allow cookies on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: CookiesAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CookiesBlockedForUrls
  #### Block cookies on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CookiesBlockedForUrls
  - GP name: Block cookies on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: CookiesBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CookiesSessionOnlyForUrls
  #### Limit cookies from specific websites to the current session
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesBlockedForUrls](#cookiesblockedforurls) policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

If you set the [RestoreOnStartup](#restoreonstartup) policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CookiesSessionOnlyForUrls
  - GP name: Limit cookies from specific websites to the current session
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: CookiesSessionOnlyForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultCookiesSetting
  #### Configure cookies
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultCookiesSetting
  - GP name: Configure cookies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultCookiesSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultCookiesSetting
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultGeolocationSetting
  #### Default geolocation setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can track users' physical locations. You can allow tracking by default (1), deny it by default (2), or ask the user each time a website requests their location (3).

If you don't configure this policy, 'AskGeolocation' policy is used and the user can change it.

* 1 = Allow sites to track users' physical location

* 2 = Don't allow any site to track users' physical location

* 3 = Ask whenever a site wants to track users' physical location

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultGeolocationSetting
  - GP name: Default geolocation setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultGeolocationSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultGeolocationSetting
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultImagesSetting
  #### Default images setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can display images. You can allow images on all sites (1) or block them on all sites (2).

If you don't configure this policy, images are allowed by default, and the user can change this setting.

* 1 = Allow all sites to show all images

* 2 = Don't allow any site to show images

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultImagesSetting
  - GP name: Default images setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultImagesSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultImagesSetting
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultInsecureContentSetting
  #### Control use of insecure content exceptions
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Allows you to set whether users can add exceptions to allow mixed content for specific sites.

This policy can be overridden for specific URL patterns using the [InsecureContentAllowedForUrls](#insecurecontentallowedforurls) and [InsecureContentBlockedForUrls](#insecurecontentblockedforurls) policies.

If this policy isn't set, users will be allowed to add exceptions to allow blockable mixed content and disable autoupgrades for optionally blockable mixed content.

* 2 = Do not allow any site to load blockable mixed content

* 3 = Allow users to add exceptions to allow blockable mixed content

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultInsecureContentSetting
  - GP name: Control use of insecure content exceptions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultInsecureContentSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DefaultInsecureContentSetting
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultJavaScriptSetting
  #### Default JavaScript setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can run JavaScript. You can allow it for all sites (1) or block it for all sites (2).

If you don't configure this policy, all sites can run JavaScript by default, and the user can change this setting.

* 1 = Allow all sites to run JavaScript

* 2 = Don't allow any site to run JavaScript

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultJavaScriptSetting
  - GP name: Default JavaScript setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultJavaScriptSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultJavaScriptSetting
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultNotificationsSetting
  #### Default notification setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can display desktop notifications. You can allow them by default (1), deny them by default (2), or have the user be asked each time a website wants to show a notification (3).

If you don't configure this policy, notifications are allowed by default, and the user can change this setting.

* 1 = Allow sites to show desktop notifications

* 2 = Don't allow any site to show desktop notifications

* 3 = Ask every time a site wants to show desktop notifications

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultNotificationsSetting
  - GP name: Default notification setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultNotificationsSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DefaultNotificationsSetting
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultPluginsSetting
  #### Default Adobe Flash setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Determines whether websites that aren't covered by [PluginsAllowedForUrls](#pluginsallowedforurls) or [PluginsBlockedForUrls](#pluginsblockedforurls) can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the [PluginsAllowedForUrls](#pluginsallowedforurls) and [PluginsBlockedForUrls](#pluginsblockedforurls) policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the [PluginsAllowedForUrls](#pluginsallowedforurls) policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the [PluginsAllowedForUrls](#pluginsallowedforurls) policy.  Existing policies using '1' will operate in Click-to-play mode.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultPluginsSetting
  - GP name: Default Adobe Flash setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultPluginsSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DefaultPluginsSetting
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultPopupsSetting
  #### Default pop-up window setting
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can show pop-up windows. You can allow them on all websites (1) or block them on all sites (2).

If you don't configure this policy, pop-up windows are blocked by default, and users can change this setting.

* 1 = Allow all sites to show pop-ups

* 2 = Don't allow any site to show pop-up windows

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultPopupsSetting
  - GP name: Default pop-up window setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultPopupsSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultPopupsSetting
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultWebBluetoothGuardSetting
  #### Control use of the Web Bluetooth API
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Control whether websites can access nearby Bluetooth devices. You can completely block access or require the site to ask the user each time it wants to access a Bluetooth device.

If you don't configure this policy, the default value (3, meaning users are asked each time) is used and users can change it.

* 2 = Don't allow any site to request access to Bluetooth devices by using the Web Bluetooth API

* 3 = Allow sites to ask the user to grant access to a nearby Bluetooth device

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultWebBluetoothGuardSetting
  - GP name: Control use of the Web Bluetooth API
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultWebBluetoothGuardSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DefaultWebBluetoothGuardSetting
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultWebUsbGuardSetting
  #### Control use of the WebUSB API
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the [WebUsbAskForUrls](#webusbaskforurls) and [WebUsbBlockedForUrls](#webusbblockedforurls) policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultWebUsbGuardSetting
  - GP name: Control use of the WebUSB API
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultWebUsbGuardSetting
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DefaultWebUsbGuardSetting
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImagesAllowedForUrls
  #### Allow images on these sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImagesAllowedForUrls
  - GP name: Allow images on these sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: ImagesAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImagesBlockedForUrls
  #### Block images on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImagesBlockedForUrls
  - GP name: Block images on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: ImagesBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### InsecureContentAllowedForUrls
  #### Allow insecure content on specified sites
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Create a list of URL patterns to specify sites that can display insecure mixed content (that is, HTTP content on HTTPS sites).

If you don't configure this policy, blockable mixed content will be blocked and optionally blockable mixed content will be upgraded. However, users will be allowed to set exceptions to allow insecure mixed content for specific sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InsecureContentAllowedForUrls
  - GP name: Allow insecure content on specified sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\1 = https://www.example.com
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\2 = [*.]example.edu

```


  #### Mac information and settings
  - Preference Key Name: InsecureContentAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### InsecureContentBlockedForUrls
  #### Block insecure content on specified sites
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Create a list of URL patterns to specify sites that aren't allowed to display blockable (i.e. active) mixed content (that is, HTTP content on HTTPS sites) and for which optionally blockable mixed content upgrades will be disabled.

If you don't configure this policy, blockable mixed content will be blocked and optionally blockable mixed content will be upgraded. However, users will be allowed to set exceptions to allow insecure mixed content for specific sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InsecureContentBlockedForUrls
  - GP name: Block insecure content on specified sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\1 = https://www.example.com
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\2 = [*.]example.edu

```


  #### Mac information and settings
  - Preference Key Name: InsecureContentBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### JavaScriptAllowedForUrls
  #### Allow JavaScript on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: JavaScriptAllowedForUrls
  - GP name: Allow JavaScript on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: JavaScriptAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### JavaScriptBlockedForUrls
  #### Block JavaScript on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: JavaScriptBlockedForUrls
  - GP name: Block JavaScript on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: JavaScriptBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Enable default legacy SameSite cookie behavior setting
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Lets you revert all cookies to legacy SameSite behavior. Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

You can set the following values for this policy:

* 1 = Revert to legacy SameSite behavior for cookies on all sites

* 2 = Use SameSite-by-default behavior for cookies on all sites

If you don't set this policy, the default behavior for cookies that don't specify a SameSite attribute will depend on other configuration sources for the SameSite-by-default feature. This feature might be set by a field trial or by enabling the same-site-by-default-cookies flag in edge://flags.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: LegacySameSiteCookieBehaviorEnabled
  - GP name: Enable default legacy SameSite cookie behavior setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: LegacySameSiteCookieBehaviorEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: LegacySameSiteCookieBehaviorEnabled
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Revert to legacy SameSite behavior for cookies on specified sites
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Cookies set for domains match specified patterns will revert to legacy SameSite behavior.

Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

If you don't set this policy, the global default value will be used. The global default will also be used for cookies on domains not covered by the patterns you specify.

The global default value can be configured using the [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) policy. If [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) is unset, the global default value falls back to other configuration sources.

Note that patterns you list in this policy are treated as domains, not URLs, so you should not specify a scheme or port.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: LegacySameSiteCookieBehaviorEnabledForDomainList
  - GP name: Revert to legacy SameSite behavior for cookies on specified sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = www.example.com
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\2 = [*.]example.edu

```


  #### Mac information and settings
  - Preference Key Name: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Example value:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NotificationsAllowedForUrls
  #### Allow notifications on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NotificationsAllowedForUrls
  - GP name: Allow notifications on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: NotificationsAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NotificationsBlockedForUrls
  #### Block notifications on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NotificationsBlockedForUrls
  - GP name: Block notifications on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: NotificationsBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PluginsAllowedForUrls
  #### Allow the Adobe Flash plug-in on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PluginsAllowedForUrls
  - GP name: Allow the Adobe Flash plug-in on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: PluginsAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PluginsBlockedForUrls
  #### Block the Adobe Flash plug-in on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PluginsBlockedForUrls
  - GP name: Block the Adobe Flash plug-in on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: PluginsBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PopupsAllowedForUrls
  #### Allow pop-up windows on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PopupsAllowedForUrls
  - GP name: Allow pop-up windows on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: PopupsAllowedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PopupsBlockedForUrls
  #### Block pop-up windows on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PopupsBlockedForUrls
  - GP name: Block pop-up windows on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: PopupsBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RegisteredProtocolHandlers
  #### Register protocol handlers
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Register a list of protocol handlers. Set the protocol property to the scheme (like 'mailto') and the url property to the URL pattern of the application that handles the scheme. The pattern can include a '%s', which will be replaced by the handled URL.

You can recommend a specific value for this policy, but you can't require that your users use it.

The protocol handlers registered by policy are merged with any handlers registered by the user, and both are available for use. The user can override the protocol handlers installed by policy by installing a new default handler, but they can't remove a protocol handler registered by policy.

  #### Supported features:
  - Can be mandatory: No
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RegisteredProtocolHandlers
  - GP name: Register protocol handlers
  - GP path (Mandatory): N/A
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Content settings
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): N/A
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: RegisteredProtocolHandlers
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Mac information and settings
  - Preference Key Name: RegisteredProtocolHandlers
  - Example value:
``` xml
<key>RegisteredProtocolHandlers</key>
<array>
  <dict>
    <key>default</key>
    <true/>
    <key>protocol</key>
    <string>mailto</string>
    <key>url</key>
    <string>https://mail.contoso.com/mail/?extsrc=mailto&url=%s</string>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebUsbAllowDevicesForUrls
  #### Grant access to specific sites to connect to specific USB devices
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to set a list of urls that specify which sites will automatically be granted permission to access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and urls in order for the policy to be valid. Each item in devices can contain a vendor ID and product ID field. Any ID that is omitted is treated as a wildcard with one exception, and that exception is that a product ID cannot be specified without a vendor ID also being specified. Otherwise, the policy will not be valid and will be ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant permission to the requesting URL to access the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Therefore, the "urls" field can contain up to two URL strings delimited by a comma to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices will be granted when the requesting site's URL matches this URL regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy will be ignored.

If this policy is left not set, the global default value will be used for all sites either from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy if it is set, or the user's personal configuration otherwise.

URL patterns in this policy should not clash with the ones configured via [WebUsbBlockedForUrls](#webusbblockedforurls). If there is a clash, this policy will take precedence over [WebUsbBlockedForUrls](#webusbblockedforurls) and [WebUsbAskForUrls](#webusbaskforurls).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebUsbAllowDevicesForUrls
  - GP name: Grant access to specific sites to connect to specific USB devices
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebUsbAllowDevicesForUrls
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAllowDevicesForUrls = [
  {
    "devices": [
      {
        "product_id": 5678, 
        "vendor_id": 1234
      }
    ], 
    "urls": [
      "https://contoso.com", 
      "https://fabrikam.com"
    ]
  }
]
```


  #### Mac information and settings
  - Preference Key Name: WebUsbAllowDevicesForUrls
  - Example value:
``` xml
<key>WebUsbAllowDevicesForUrls</key>
<array>
  <dict>
    <key>devices</key>
    <array>
      <dict>
        <key>product_id</key>
        <integer>5678</integer>
        <key>vendor_id</key>
        <integer>1234</integer>
      </dict>
    </array>
    <key>urls</key>
    <array>
      <string>https://contoso.com</string>
      <string>https://fabrikam.com</string>
    </array>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebUsbAskForUrls
  #### Allow WebUSB on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the [WebUsbBlockedForUrls](#webusbblockedforurls) policy - you can't both allow and block a URL.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebUsbAskForUrls
  - GP name: Allow WebUSB on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: WebUsbAskForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebUsbBlockedForUrls
  #### Block WebUSB on specific sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the [WebUsbAskForUrls](#webusbaskforurls) policy. You can't both allow and block a URL.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebUsbBlockedForUrls
  - GP name: Block WebUSB on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: WebUsbBlockedForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Default search provider policies

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderEnabled
  #### Enable the default search provider
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables the ability to use a default search provider.

If you enable this policy, a user can search for a term by typing in the address bar (as long as what they type isn't a URL).

You can specify the default search provider to use by enabling the rest of the default search policies. If these are left empty (not configured) or configured incorrectly, the user can choose the default provider.

If you disable this policy, the user can't search from the address bar.

If you enable or disable this policy, users can't change or override it.

If you don't configure this policy, the default search provider is enabled, and the user can choose the default search provider and set the search provider list.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderEnabled
  - GP name: Enable the default search provider
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderEncodings
  #### Default search provider encodings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderEncodings
  - GP name: Default search provider encodings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = UTF-8
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = UTF-16
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = GB2312
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\4 = ISO-8859-1

```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderEncodings
  - Example value:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderImageURL
  #### Specifies the search-by-image feature for the default search provider
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

Specify Bing's Image Search URL as:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Specify Google's Image Search URL as: '{google:baseURL}searchbyimage/upload'.

See [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) policy to finish configuring image search.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderImageURL
  - GP name: Specifies the search-by-image feature for the default search provider
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderImageURL
  - Value Type: REG_SZ
  ##### Example value:
```
https://search.contoso.com/searchbyimage/upload
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderImageURL
  - Example value:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderImageURLPostParams
  #### Parameters for an image URL that uses POST
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

Specify Bing's Image Search URL Post Params as:
'imageBin={google:imageThumbnailBase64}'.

Specify Google's Image Search URL Post Params as:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderImageURLPostParams
  - GP name: Parameters for an image URL that uses POST
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderImageURLPostParams
  - Value Type: REG_SZ
  ##### Example value:
```
content={imageThumbnail},url={imageURL},sbisrc={SearchSource}
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderImageURLPostParams
  - Example value:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderKeyword
  #### Default search provider keyword
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderKeyword
  - GP name: Default search provider keyword
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderKeyword
  - Value Type: REG_SZ
  ##### Example value:
```
mis
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderKeyword
  - Example value:
``` xml
<string>mis</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderName
  #### Default search provider name
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderName
  - GP name: Default search provider name
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderName
  - Value Type: REG_SZ
  ##### Example value:
```
My Intranet Search
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderName
  - Example value:
``` xml
<string>My Intranet Search</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderSearchURL
  #### Default search provider search URL
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) policy; if you don't enable the latter policy, this policy is ignored.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderSearchURL
  - GP name: Default search provider search URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderSearchURL
  - Value Type: REG_SZ
  ##### Example value:
```
https://search.contoso.com/search?q={searchTerms}
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderSearchURL
  - Example value:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultSearchProviderSuggestURL
  #### Default search provider URL for suggestions
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderSuggestURL
  - GP name: Default search provider URL for suggestions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultSearchProviderSuggestURL
  - Value Type: REG_SZ
  ##### Example value:
```
https://search.contoso.com/suggest?q={searchTerms}
```


  #### Mac information and settings
  - Preference Key Name: DefaultSearchProviderSuggestURL
  - Example value:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Extensions policies

  [Back to top](#microsoft-edge---policies)

  ### ExtensionAllowedTypes
  #### Configure allowed extension types
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using [ExtensionInstallForcelist](#extensioninstallforcelist) policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionAllowedTypes
  - GP name: Configure allowed extension types
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\1 = hosted_app

```


  #### Mac information and settings
  - Preference Key Name: ExtensionAllowedTypes
  - Example value:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExtensionInstallAllowlist
  #### Allow specific extensions to be installed
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  By default, all extensions are allowed. However, if you block all extensions by setting the 'ExtensionInstallBlockList' policy to "*," users can only install extensions defined in this policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallAllowlist
  - GP name: Allow specific extensions to be installed
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = extension_id1
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\2 = extension_id2

```


  #### Mac information and settings
  - Preference Key Name: ExtensionInstallAllowlist
  - Example value:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExtensionInstallBlocklist
  #### Control which extensions cannot be installed
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  List specific extensions that users can NOT install in Microsoft Edge. When you deploy this policy, any extensions on this list that were previously installed will be disabled, and the user won't be able to enable them. If you remove an item from the list of blocked extensions, that extension is automatically re-enabled anywhere it was previously installed.

Use "*" to block all extensions that aren't explicitly listed in the allow list.

If you don't configure this policy, users can install any extension in Microsoft Edge.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallBlocklist
  - GP name: Control which extensions cannot be installed
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = extension_id1
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\2 = extension_id2

```


  #### Mac information and settings
  - Preference Key Name: ExtensionInstallBlocklist
  - Example value:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExtensionInstallForcelist
  #### Control which extensions are installed silently
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies extensions that are installed silently, without user interaction, and that the users can't uninstall or disable ("force-installed"). All permissions requested by the extensions are granted implicitly, without user interaction, including any additional permissions requested by future versions of the extension. Furthermore, permissions are granted for the enterprise.deviceAttributes and enterprise.platformKeys extension APIs. (These two APIs are only available to extensions that are force-installed.)

This policy takes precedence over a potentially conflicting [ExtensionInstallBlocklist](#extensioninstallblocklist) policy. When you take an extension off of the force-installed list it's automatically uninstalled by Microsoft Edge.

For Windows devices that aren't joined to a Microsoft Active Directory domain, forced installation is limited to extensions available in the Microsoft Store.

Note that users can modify the source code of any extension by using Developer Tools, potentially rendering the extension dysfunctional. If this is a concern, set the [DeveloperToolsAvailability](#developertoolsavailability) policy.

Use the following format to add an extension to the list:

[extensionID];[updateURL]

- extensionID - the 32-letter string found on edge://extensions when in developer mode.

- updateURL (optional) is the address of the Update Manifest XML document for the app or extension, as described at [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043). If you don't set the updateURL, the Microsoft Store update URL is used (currently https://edge.microsoft.com/extensionwebstorebase/v1/crx).  Note that the update URL set in this policy is only used for the initial installation; subsequent updates of the extension use the update URL indicated in the extension's manifest.

For example, gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx installs the Microsoft Online app from the Microsoft Store "update" URL. For more information about hosting extensions, see: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044).

If you don't configure this policy, no extensions are installed automatically, and users can uninstall any extension in Microsoft Edge.

Note that this policy doesn't apply to InPrivate mode.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallForcelist
  - GP name: Control which extensions are installed silently
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\2 = abcdefghijklmnopabcdefghijklmnop

```


  #### Mac information and settings
  - Preference Key Name: ExtensionInstallForcelist
  - Example value:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExtensionInstallSources
  #### Configure extension and user script install sources
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The [ExtensionInstallBlocklist](#extensioninstallblocklist) policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallSources
  - GP name: Configure extension and user script install sources
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\1 = https://corp.contoso.com/*

```


  #### Mac information and settings
  - Preference Key Name: ExtensionInstallSources
  - Example value:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExtensionSettings
  #### Configure extension management settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures extension management settings for Microsoft Edge.

This policy controls multiple settings, including settings controlled by any existing extension-related policies. This policy overrides any legacy policies if both are set.

This policy maps an extension ID or an update URL to its configuration. With an extension ID, the configuration is applied only to the specified extension. Set a default configuration for the special ID "*", to apply to all extensions that aren't specifically listed in this policy. With an update URL, the configuration is applied to all extensions with the exact update URL stated in manifest of this extension, as described at [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExtensionSettings
  - GP name: Configure extension management settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ExtensionSettings
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionSettings = {
  "*": {
    "allowed_types": [
      "hosted_app"
    ], 
    "blocked_install_message": "Custom error message.", 
    "blocked_permissions": [
      "downloads", 
      "bookmarks"
    ], 
    "install_sources": [
      "https://company-intranet/apps"
    ], 
    "installation_mode": "blocked", 
    "runtime_allowed_hosts": [
      "*://good.contoso.com"
    ], 
    "runtime_blocked_hosts": [
      "*://*.contoso.com"
    ]
  }, 
  "abcdefghijklmnopabcdefghijklmnop": {
    "blocked_permissions": [
      "history"
    ], 
    "installation_mode": "allowed", 
    "minimum_version_required": "1.0.1"
  }, 
  "bcdefghijklmnopabcdefghijklmnopa": {
    "allowed_permissions": [
      "downloads"
    ], 
    "installation_mode": "force_installed", 
    "runtime_allowed_hosts": [
      "*://good.contoso.com"
    ], 
    "runtime_blocked_hosts": [
      "*://*.contoso.com"
    ], 
    "update_url": "https://contoso.com/update_url"
  }, 
  "cdefghijklmnopabcdefghijklmnopab": {
    "blocked_install_message": "Custom error message.", 
    "installation_mode": "blocked"
  }, 
  "defghijklmnopabcdefghijklmnopabc,efghijklmnopabcdefghijklmnopabcd": {
    "blocked_install_message": "Custom error message.", 
    "installation_mode": "blocked"
  }, 
  "fghijklmnopabcdefghijklmnopabcde": {
    "blocked_install_message": "Custom removal message.", 
    "installation_mode": "removed"
  }, 
  "update_url:https://www.contoso.com/update.xml": {
    "allowed_permissions": [
      "downloads"
    ], 
    "blocked_permissions": [
      "wallpaper"
    ], 
    "installation_mode": "allowed"
  }
}
```


  #### Mac information and settings
  - Preference Key Name: ExtensionSettings
  - Example value:
``` xml
<key>ExtensionSettings</key>
<dict>
  <key>*</key>
  <dict>
    <key>allowed_types</key>
    <array>
      <string>hosted_app</string>
    </array>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>blocked_permissions</key>
    <array>
      <string>downloads</string>
      <string>bookmarks</string>
    </array>
    <key>install_sources</key>
    <array>
      <string>https://company-intranet/apps</string>
    </array>
    <key>installation_mode</key>
    <string>blocked</string>
    <key>runtime_allowed_hosts</key>
    <array>
      <string>*://good.contoso.com</string>
    </array>
    <key>runtime_blocked_hosts</key>
    <array>
      <string>*://*.contoso.com</string>
    </array>
  </dict>
  <key>abcdefghijklmnopabcdefghijklmnop</key>
  <dict>
    <key>blocked_permissions</key>
    <array>
      <string>history</string>
    </array>
    <key>installation_mode</key>
    <string>allowed</string>
    <key>minimum_version_required</key>
    <string>1.0.1</string>
  </dict>
  <key>bcdefghijklmnopabcdefghijklmnopa</key>
  <dict>
    <key>allowed_permissions</key>
    <array>
      <string>downloads</string>
    </array>
    <key>installation_mode</key>
    <string>force_installed</string>
    <key>runtime_allowed_hosts</key>
    <array>
      <string>*://good.contoso.com</string>
    </array>
    <key>runtime_blocked_hosts</key>
    <array>
      <string>*://*.contoso.com</string>
    </array>
    <key>update_url</key>
    <string>https://contoso.com/update_url</string>
  </dict>
  <key>cdefghijklmnopabcdefghijklmnopab</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>installation_mode</key>
    <string>blocked</string>
  </dict>
  <key>defghijklmnopabcdefghijklmnopabc,efghijklmnopabcdefghijklmnopabcd</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>installation_mode</key>
    <string>blocked</string>
  </dict>
  <key>fghijklmnopabcdefghijklmnopabcde</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom removal message.</string>
    <key>installation_mode</key>
    <string>removed</string>
  </dict>
  <key>update_url:https://www.contoso.com/update.xml</key>
  <dict>
    <key>allowed_permissions</key>
    <array>
      <string>downloads</string>
    </array>
    <key>blocked_permissions</key>
    <array>
      <string>wallpaper</string>
    </array>
    <key>installation_mode</key>
    <string>allowed</string>
  </dict>
</dict>
```
  

  [Back to top](#microsoft-edge---policies)

  ## HTTP authentication policies

  [Back to top](#microsoft-edge---policies)

  ### AllowCrossOriginAuthPrompt
  #### Allow cross-origin HTTP Basic Auth prompts
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Controls whether third-party sub-content on a page can open an HTTP Basic Auth dialog box.

Typically, this is disabled as a phishing defense. If you don't configure this policy, it's disabled and third-party sub-content can't open a HTTP Basic Auth dialog box.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowCrossOriginAuthPrompt
  - GP name: Allow cross-origin HTTP Basic Auth prompts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowCrossOriginAuthPrompt
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AllowCrossOriginAuthPrompt
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AuthNegotiateDelegateAllowlist
  #### Specifies a list of servers that Microsoft Edge can delegate user credentials to
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configure the list of servers that Microsoft Edge can delegate to.

Separate multiple server names with commas. Wildcards (*) are allowed.

If you don't configure this policy Microsoft Edge won't delegate user credentials even if a server is detected as Intranet.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AuthNegotiateDelegateAllowlist
  - GP name: Specifies a list of servers that Microsoft Edge can delegate user credentials to
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AuthNegotiateDelegateAllowlist
  - Value Type: REG_SZ
  ##### Example value:
```
contoso.com
```


  #### Mac information and settings
  - Preference Key Name: AuthNegotiateDelegateAllowlist
  - Example value:
``` xml
<string>contoso.com</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AuthSchemes
  #### Supported authentication schemes
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies which HTTP authentication schemes are supported.

You can configure the policy by using these values: 'basic', 'digest', 'ntlm', and 'negotiate'. Separate multiple values with commas.

If you don't configure this policy, all four schemes are used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AuthSchemes
  - GP name: Supported authentication schemes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AuthSchemes
  - Value Type: REG_SZ
  ##### Example value:
```
basic,digest,ntlm,negotiate
```


  #### Mac information and settings
  - Preference Key Name: AuthSchemes
  - Example value:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AuthServerAllowlist
  #### Configure list of allowed authentication servers
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies which servers to enable for integrated authentication. Integrated authentication is only enabled when Microsoft Edge receives an authentication challenge from a proxy or from a server in this list.

Separate multiple server names with commas. Wildcards (*) are allowed.

If you don't configure this policy, Microsoft Edge tries to detect if a server is on the intranet - only then will it respond to IWA requests. If the server is on the internet, IWA requests from it are ignored by Microsoft Edge.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AuthServerAllowlist
  - GP name: Configure list of allowed authentication servers
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AuthServerAllowlist
  - Value Type: REG_SZ
  ##### Example value:
```
*contoso.com,contoso.com
```


  #### Mac information and settings
  - Preference Key Name: AuthServerAllowlist
  - Example value:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DisableAuthNegotiateCnameLookup
  #### Disable CNAME lookup when negotiating Kerberos authentication
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Determines whether the generated Kerberos SPN is based on the canonical DNS name (CNAME) or on the original name entered.

If you enable this policy, CNAME lookup is skipped and the server name (as entered) is used.

If you disable this policy or don't configure it, the canonical name of the server is used.  This is determined through CNAME lookup.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DisableAuthNegotiateCnameLookup
  - GP name: Disable CNAME lookup when negotiating Kerberos authentication
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DisableAuthNegotiateCnameLookup
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: DisableAuthNegotiateCnameLookup
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EnableAuthNegotiatePort
  #### Include non-standard port in Kerberos SPN
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies whether the generated Kerberos SPN should include a non-standard port.

If you enable this policy, and a user includes a non-standard port (a port other than 80 or 443) in a URL, that port is included in the generated Kerberos SPN.

If you don't configure or disable this policy, the generated Kerberos SPN won't include a port in any case.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnableAuthNegotiatePort
  - GP name: Include non-standard port in Kerberos SPN
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EnableAuthNegotiatePort
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: EnableAuthNegotiatePort
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NtlmV2Enabled
  #### Control whether NTLMv2 authentication is enabled
  
  #### Supported versions:
  - On macOS since 77 or later

  #### Description
  Controls whether NTLMv2 is enabled.

All recent versions of Samba and Windows servers support NTLMv2. You should only disable NTLMv2 to address issues with backwards compatibility as it reduces the security of authentication.

If you don't configure this policy, NTLMv2 is enabled by default.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  

  #### Mac information and settings
  - Preference Key Name: NtlmV2Enabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Native Messaging policies

  [Back to top](#microsoft-edge---policies)

  ### NativeMessagingAllowlist
  #### Control which native messaging hosts users can use
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the [NativeMessagingBlocklist](#nativemessagingblocklist) policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NativeMessagingAllowlist
  - GP name: Control which native messaging hosts users can use
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = com.native.messaging.host.name1
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\2 = com.native.messaging.host.name2

```


  #### Mac information and settings
  - Preference Key Name: NativeMessagingAllowlist
  - Example value:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NativeMessagingBlocklist
  #### Configure native messaging block list
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies which native messaging hosts that shouldn't be used.

Use '*' to block all native messaging hosts unless they are explicitly listed in the allow list.

If you don't configure this policy, Microsoft Edge will load all installed native messaging hosts.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NativeMessagingBlocklist
  - GP name: Configure native messaging block list
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = com.native.messaging.host.name1
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\2 = com.native.messaging.host.name2

```


  #### Mac information and settings
  - Preference Key Name: NativeMessagingBlocklist
  - Example value:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NativeMessagingUserLevelHosts
  #### Allow user-level native messaging hosts (installed without admin permissions)
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables user-level installation of native messaging hosts.

If you disable this policy, Microsoft Edge will only use native messaging hosts installed on the system level.

By default, if you don't configure this policy, Microsoft Edge will allow usage of user-level native messaging hosts.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NativeMessagingUserLevelHosts
  - GP name: Allow user-level native messaging hosts (installed without admin permissions)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: NativeMessagingUserLevelHosts
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: NativeMessagingUserLevelHosts
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Password manager and protection policies

  [Back to top](#microsoft-edge---policies)

  ### PasswordManagerEnabled
  #### Enable saving passwords to the password manager
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enable Microsoft Edge to save user passwords.

If you enable this policy, users can save their passwords in Microsoft Edge. The next time they visit the site, Microsoft Edge will enter the password automatically.

If you disable this policy, users can't save new passwords, but they can still use previously saved passwords.

If you enable or disable this policy, users can't change or override it in Microsoft Edge. If you don't configure it, users can save passwords, as well as turn this feature off.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PasswordManagerEnabled
  - GP name: Enable saving passwords to the password manager
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Password manager and protection
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: PasswordManagerEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PasswordManagerEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PasswordProtectionChangePasswordURL
  #### Configure the change password URL
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the change password URL (HTTP and HTTPS schemes only).

Password protection service will send users to this URL to change their password after seeing a warning in the browser.

If you enable this policy, then password protection service sends users to this URL to change their password.

If you disable this policy or don't configure it, then password protection service will not redirect users to a change password URL.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionChangePasswordURL
  - GP name: Configure the change password URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PasswordProtectionChangePasswordURL
  - Value Type: REG_SZ
  ##### Example value:
```
https://contoso.com/change_password.html
```


  #### Mac information and settings
  - Preference Key Name: PasswordProtectionChangePasswordURL
  - Example value:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PasswordProtectionLoginURLs
  #### Configure the list of enterprise login URLs where password protection service should capture fingerprint of password
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configure the list of enterprise login URLs (HTTP and HTTPS schemes only) where Microsoft Edge should capture the fingerprint of passwords and use it for password reuse detection.

If you enable this policy, the password protection service captures fingerprints of passwords on the defined URLs.

If you disable this policy or don't configure it, no password fingerprints are captured.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionLoginURLs
  - GP name: Configure the list of enterprise login URLs where password protection service should capture fingerprint of password
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = https://contoso.com/login.html
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\2 = https://login.contoso.com

```


  #### Mac information and settings
  - Preference Key Name: PasswordProtectionLoginURLs
  - Example value:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PasswordProtectionWarningTrigger
  #### Configure password protection warning trigger
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), as well as for the sites listed in [SmartScreenAllowListDomains](#smartscreenallowlistdomains), will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-allowlisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionWarningTrigger
  - GP name: Configure password protection warning trigger
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PasswordProtectionWarningTrigger
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PasswordProtectionWarningTrigger
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Printing policies

  [Back to top](#microsoft-edge---policies)

  ### DefaultPrinterSelection
  #### Default printer selection rules
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Overrides Microsoft Edge default printer selection rules. This policy determines the rules for selecting the default printer in Microsoft Edge, which happens the first time a user tries to print a page.

When this policy is set, Microsoft Edge tries to find a printer that matches all of the specified attributes and uses it as default printer. If there are multiple printers that meet the criteria, the first printer that matches is used.

If you don't configure this policy or no matching printers are found within the timeout, the printer defaults to the built-in PDF printer or no printer, if the PDF printer isn't available.

The value is parsed as a JSON object, conforming to the following schema: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

Omitting a field means all values match; for example, if you don't specify connectivity Print Preview starts discovering all kinds of local printers. Regular expression patterns must follow the JavaScript RegExp syntax and matches are case sensitive.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultPrinterSelection
  - GP name: Default printer selection rules
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultPrinterSelection
  - Value Type: REG_SZ
  ##### Example value:
```
{ "idPattern": ".*public", "namePattern": ".*Color" }
```


  #### Mac information and settings
  - Preference Key Name: DefaultPrinterSelection
  - Example value:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PrintHeaderFooter
  #### Print headers and footers
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Force 'headers and footers' to be on or off in the printing dialog.

If you don't configure this policy, users can decide whether to print headers and footers.

If you disable this policy, users can't print headers and footers.

If you enable this policy, users always print headers and footers.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PrintHeaderFooter
  - GP name: Print headers and footers
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Printing
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: PrintHeaderFooter
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: PrintHeaderFooter
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Set the system default printer as the default printer
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Tells Microsoft Edge to use the system default printer as the default choice in Print Preview instead of the most recently used printer.

If you disable this policy or don't configure it, Print Preview uses the most recently used printer as the default destination choice.

If you enable this policy, Print Preview uses the OS system default printer as the default destination choice.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PrintPreviewUseSystemDefaultPrinter
  - GP name: Set the system default printer as the default printer
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Printing
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: PrintPreviewUseSystemDefaultPrinter
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: PrintPreviewUseSystemDefaultPrinter
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PrintingEnabled
  #### Enable printing
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables printing in Microsoft Edge and prevents users from changing this setting.

If you enable this policy or don't configure it, users can print.

If you disable this policy, users can't print from Microsoft Edge. Printing is disabled in the wrench menu, extensions, JavaScript applications, and so on. Users can still print from plug-ins that bypass Microsoft Edge while printing. For example, certain Adobe Flash applications have the print option in their context menu, which isn't covered by this policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PrintingEnabled
  - GP name: Enable printing
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PrintingEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PrintingEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### UseSystemPrintDialog
  #### Print using system print dialog
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Shows the system print dialog instead of print preview.

If you enable this policy, Microsoft Edge opens the system print dialog instead of the built-in print preview when a user prints a page.

If you don't configure or disable this policy, print commands trigger the Microsoft Edge print preview screen.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: UseSystemPrintDialog
  - GP name: Print using system print dialog
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: UseSystemPrintDialog
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: UseSystemPrintDialog
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Proxy server policies

  [Back to top](#microsoft-edge---policies)

  ### ProxyBypassList
  #### Configure proxy bypass rules
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProxyBypassList
  - GP name: Configure proxy bypass rules
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProxyBypassList
  - Value Type: REG_SZ
  ##### Example value:
```
https://www.contoso.com, https://www.fabrikam.com
```


  #### Mac information and settings
  - Preference Key Name: ProxyBypassList
  - Example value:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ProxyMode
  #### Configure proxy server settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify the proxy server settings used by Microsoft Edge. If you enable this policy, users can't change the proxy settings.

If you choose to never use a proxy server and to always connect directly, all other options are ignored.

If you choose to use system proxy settings, all other options are ignored.

If you choose to auto detect the proxy server, all other options are ignored.

If you choose fixed server proxy mode, you can specify further options in [ProxyServer](#proxyserver) and 'Comma-separated list of proxy bypass rules'.

If you choose to use a .pac proxy script, you must specify the URL to the script in 'URL to a proxy .pac file'.

For detailed examples, go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

If you enable this policy, Microsoft Edge will ignore all proxy-related options specified from the command line.

If you don't configure this policy users can choose their own proxy settings.

* "direct" = Never use a proxy

* "auto_detect" = Auto detect proxy settings

* "pac_script" = Use a .pac proxy script

* "fixed_servers" = Use fixed proxy servers

* "system" = Use system proxy settings

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProxyMode
  - GP name: Configure proxy server settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProxyMode
  - Value Type: REG_SZ
  ##### Example value:
```
direct
```


  #### Mac information and settings
  - Preference Key Name: ProxyMode
  - Example value:
``` xml
<string>direct</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ProxyPacUrl
  #### Set the proxy .pac file URL
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProxyPacUrl
  - GP name: Set the proxy .pac file URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProxyPacUrl
  - Value Type: REG_SZ
  ##### Example value:
```
https://internal.contoso.com/example.pac
```


  #### Mac information and settings
  - Preference Key Name: ProxyPacUrl
  - Example value:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ProxyServer
  #### Configure address or URL of proxy server
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProxyServer
  - GP name: Configure address or URL of proxy server
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProxyServer
  - Value Type: REG_SZ
  ##### Example value:
```
123.123.123.123:8080
```


  #### Mac information and settings
  - Preference Key Name: ProxyServer
  - Example value:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ProxySettings
  #### Proxy settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the proxy settings for Microsoft Edge.

If you enable this policy, Microsoft Edge ignores all proxy-related options specified from the command line.

If you don't configure this policy, users can choose their own proxy settings.

This policy overrides the following individual policies:

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

The ProxyMode field lets you specify the proxy server used by Microsoft Edge and prevents users from changing proxy settings.

The ProxyPacUrl field is a URL to a proxy .pac file.

The ProxyServer field is a URL for the proxy server.

The ProxyBypassList field is a list of proxy hosts that Microsoft Edge bypasses.

If you choose the 'direct' value as 'ProxyMode', a proxy is never used and all other fields are ignored.

If you choose the 'system' value as 'ProxyMode', the systems's proxy is used and all other fields are ignored.

If you choose the 'auto_detect' value as 'ProxyMode', all other fields are ignored.

If you choose the 'fixed_server' value as 'ProxyMode', the 'ProxyServer' and 'ProxyBypassList' fields are used.

If you choose the 'pac_script' value as 'ProxyMode', the 'ProxyPacUrl' and 'ProxyBypassList' fields are used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProxySettings
  - GP name: Proxy settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProxySettings
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Mac information and settings
  - Preference Key Name: ProxySettings
  - Example value:
``` xml
<key>ProxySettings</key>
<dict>
  <key>ProxyBypassList</key>
  <string>https://www.example1.com,https://www.example2.com,https://internalsite/</string>
  <key>ProxyMode</key>
  <string>direct</string>
  <key>ProxyPacUrl</key>
  <string>https://internal.site/example.pac</string>
  <key>ProxyServer</key>
  <string>123.123.123.123:8080</string>
</dict>
```
  

  [Back to top](#microsoft-edge---policies)

  ## SmartScreen settings policies

  [Back to top](#microsoft-edge---policies)

  ### PreventSmartScreenPromptOverride
  #### Prevent bypassing Microsoft Defender SmartScreen prompts for sites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PreventSmartScreenPromptOverride
  - GP name: Prevent bypassing Microsoft Defender SmartScreen prompts for sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PreventSmartScreenPromptOverride
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PreventSmartScreenPromptOverride
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads
  
  #### Supported versions:
  - On Windows since 77 or later
  - On macOS since 79 or later

  #### Description
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PreventSmartScreenPromptOverrideForFiles
  - GP name: Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PreventSmartScreenPromptOverrideForFiles
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PreventSmartScreenPromptOverrideForFiles
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SmartScreenAllowListDomains
  #### Configure the list of domains for which Microsoft Defender SmartScreen won't trigger warnings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configure the list of Microsoft Defender SmartScreen trusted domains. This means:
Microsoft Defender SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The Microsoft Defender SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, Microsoft Defender SmartScreen trusts these domains.
If you disable or don't set this policy, default Microsoft Defender SmartScreen protection is applied to all resources.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SmartScreenAllowListDomains
  - GP name: Configure the list of domains for which Microsoft Defender SmartScreen won't trigger warnings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = mydomain.com
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\2 = myuniversity.edu

```


  #### Mac information and settings
  - Preference Key Name: SmartScreenAllowListDomains
  - Example value:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SmartScreenEnabled
  #### Configure Microsoft Defender SmartScreen
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SmartScreenEnabled
  - GP name: Configure Microsoft Defender SmartScreen
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: SmartScreenEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SmartScreenEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Force Microsoft Defender SmartScreen checks on downloads from trusted sources
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  This policy setting lets you configure whether Microsoft Defender SmartScreen checks download reputation from a trusted source.

If you enable or don't configure this setting, Microsoft Defender SmartScreen checks the download’s reputation regardless of source.

If you disable this setting, Microsoft Defender SmartScreen doesn’t check the download’s reputation when downloading from a trusted source.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SmartScreenForTrustedDownloadsEnabled
  - GP name: Force Microsoft Defender SmartScreen checks on downloads from trusted sources
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: SmartScreenForTrustedDownloadsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### SmartScreenPuaEnabled
  #### Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  This policy setting lets you configure whether to turn on blocking for potentially unwanted apps with Microsoft Defender SmartScreen. Potentially unwanted app blocking with Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking with Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking with Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking with Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking with Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SmartScreenPuaEnabled
  - GP name: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: SmartScreenPuaEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SmartScreenPuaEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Startup&comma; home page and new tab page policies

  [Back to top](#microsoft-edge---policies)

  ### HomepageIsNewTabPage
  #### Set the new tab page as the home page
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the default home page in Microsoft Edge. You can set the home page to a URL you specify or to the new tab page.

If you enable this policy, the new tab page is always used for the home page, and the home page URL location is ignored.

If you disable this policy, the user's home page can't be the new tab page, unless the URL is set to 'edge://newtab'.

If not configured users can choose whether the new tab page is their home page.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: HomepageIsNewTabPage
  - GP name: Set the new tab page as the home page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: HomepageIsNewTabPage
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: HomepageIsNewTabPage
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### HomepageLocation
  #### Configure the home page URL
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the [RestoreOnStartup](#restoreonstartup) policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the [HomepageIsNewTabPage](#homepageisnewtabpage) policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: HomepageLocation
  - GP name: Configure the home page URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: HomepageLocation
  - Value Type: REG_SZ
  ##### Example value:
```
https://www.contoso.com
```


  #### Mac information and settings
  - Preference Key Name: HomepageLocation
  - Example value:
``` xml
<string>https://www.contoso.com</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NewTabPageCompanyLogo
  #### Set new tab page company logo
  >DEPRECATED: This policy is deprecated. It is currently supported but will become obsolete in a future release.
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  We are deprecating this policy because it doesn't work as expected and recommend that it not be used.

Specifies the company logo to use on the new tab page in Microsoft Edge.

The policy should be configured as a string that expresses the logo(s) in JSON format. For example: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

You configure this policy by specifying the URL from which Microsoft Edge can download the logo and its cryptographic hash (SHA-256), which is used to verify the integrity of the download. The logo must be in PNG or SVG format, and its file size must not exceed 16 MB. The logo is downloaded and cached, and it will be redownloaded whenever the URL or the hash changes. The URL must be accessible without any authentication.

The 'default_logo' is required and will be used when there's no background image. If 'light_logo' is provided, it will be used when the user's new tab page has a background image. We recommend a horizontal logo with a transparent background that is left-aligned and vertically centered. The logo should have a minimum height of 32 pixels and an aspect ratio from 1:1 to 4:1. The 'default_logo' should have proper contrast against a white/black background while the 'light_logo' should have proper contrast against a background image.

If you enable this policy, Microsoft Edge downloads and shows the specified logo(s) on the new tab page. Users can't override or hide the logo(s).

If you disable or don't configure this policy, Microsoft Edge will show no company logo or a Microsoft logo on the new tab page.

For help with determining the SHA-256 hash, see https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NewTabPageCompanyLogo
  - GP name: Set new tab page company logo %s(deprecated)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: NewTabPageCompanyLogo
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NewTabPageCompanyLogo = {
  "default_logo": {
    "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29", 
    "url": "https://www.contoso.com/logo.png"
  }, 
  "light_logo": {
    "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737", 
    "url": "https://www.contoso.com/light_logo.png"
  }
}
```


  #### Mac information and settings
  - Preference Key Name: NewTabPageCompanyLogo
  - Example value:
``` xml
<key>NewTabPageCompanyLogo</key>
<dict>
  <key>default_logo</key>
  <dict>
    <key>hash</key>
    <string>cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29</string>
    <key>url</key>
    <string>https://www.contoso.com/logo.png</string>
  </dict>
  <key>light_logo</key>
  <dict>
    <key>hash</key>
    <string>517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737</string>
    <key>url</key>
    <string>https://www.contoso.com/light_logo.png</string>
  </dict>
</dict>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NewTabPageHideDefaultTopSites
  #### Hide the default top sites from the new tab page
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Hides the default top sites from the new tab page in Microsoft Edge.

If you set this policy to true, the default top site tiles are hidden.

If you set this policy to false or don't configure it, the default top site tiles remain visible.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NewTabPageHideDefaultTopSites
  - GP name: Hide the default top sites from the new tab page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: NewTabPageHideDefaultTopSites
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: NewTabPageHideDefaultTopSites
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NewTabPageLocation
  #### Configure the new tab page URL
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the [RestoreOnStartup](#restoreonstartup) policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the [NewTabPageSetFeedType](#newtabpagesetfeedtype) policy, this policy has precedence.

If an invalid URL is provided, new tabs will open about://blank.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NewTabPageLocation
  - GP name: Configure the new tab page URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: NewTabPageLocation
  - Value Type: REG_SZ
  ##### Example value:
```
https://www.fabrikam.com
```


  #### Mac information and settings
  - Preference Key Name: NewTabPageLocation
  - Example value:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NewTabPageManagedQuickLinks
  #### Set new tab page quick links
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  By default, Microsoft Edge displays quick links on the new tab page from user-added shortcuts and top sites based on browsing history. With this policy, you can configure up to three quick link tiles on the new tab page, expressed as a JSON object:

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

The 'url' field is required; 'title' and 'pinned' are optional. If 'title' is not provided, the URL is used as the default title. If 'pinned' is not provided, the default value is false.

Microsoft Edge presents these in the order listed, from left to right, with all pinned tiles displayed ahead of non-pinned tiles.

If the policy is set as mandatory, the 'pinned' field will be ignored and all tiles will be pinned. The tiles can't be deleted by the user and will always appear at the front of the quick links list.

If the policy is set as recommended, pinned tiles will remain in the list but the user has the ability to edit and delete them. Quick link tiles that aren't pinned behave like default top sites and are pushed off the list if other websites are visited more frequently. When applying non-pinned links via this policy to an existing browser profile, the links may not appear at all, depending on how they rank compared to the user's browsing history.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NewTabPageManagedQuickLinks
  - GP name: Set new tab page quick links
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: NewTabPageManagedQuickLinks
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\NewTabPageManagedQuickLinks = [
  {
    "pinned": true, 
    "title": "Contoso Portal", 
    "url": "https://contoso.com"
  }, 
  {
    "title": "Fabrikam", 
    "url": "https://fabrikam.com"
  }
]
```


  #### Mac information and settings
  - Preference Key Name: NewTabPageManagedQuickLinks
  - Example value:
``` xml
<key>NewTabPageManagedQuickLinks</key>
<array>
  <dict>
    <key>pinned</key>
    <true/>
    <key>title</key>
    <string>Contoso Portal</string>
    <key>url</key>
    <string>https://contoso.com</string>
  </dict>
  <dict>
    <key>title</key>
    <string>Fabrikam</string>
    <key>url</key>
    <string>https://fabrikam.com</string>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NewTabPageSetFeedType
  #### Configure the Microsoft Edge new tab page experience
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Lets you choose either the Microsoft News or Office 365 feed experience for the new tab page.

When you set this policy to Microsoft News feed experience (0), users will see the Microsoft News feed experience on the new tab page.

When you set this policy to Office 365 feed experience (1), users with an Azure Active Directory browser sign-in will see the Office 365 feed experience on the new tab page.

If you disable or don't configure this policy:

- Users with an Azure Active Directory browser sign-in are offered the Office 365 new tab page feed experience, as well as the standard new tab page feed experience.

- Users without an Azure Active Directory browser sign-in will see the standard new tab page experience.

If you configure this policy *and* the [NewTabPageLocation](#newtabpagelocation) policy, [NewTabPageLocation](#newtabpagelocation) has precedence.

Default setting:  Disabled or not configured.

* 0 = Microsoft News feed experience

* 1 = Office 365 feed experience

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NewTabPageSetFeedType
  - GP name: Configure the Microsoft Edge new tab page experience
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: NewTabPageSetFeedType
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: NewTabPageSetFeedType
  - Example value:
``` xml
<integer>0</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RestoreOnStartup
  #### Action to take on startup
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify how Microsoft Edge behaves when it starts.

If you want a new tab to always open on startup, choose 'Open new tab' (5).

If you want to reopen URLs that were open the last time Microsoft Edge closed, choose 'Restore the last session' (1). The browsing session will be restored as it was. Note that this option disables some settings that rely on sessions or that perform actions on exit (such as Clear browsing data on exit or session-only cookies).

If you want to open a specific set of URLs, choose 'Open a list of URLs' (4).

Disabling this setting is equivalent to leaving it not configured. Users will be able to change it in Microsoft Edge.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

	 

* 1 = Restore the last session

* 4 = Open a list of URLs

* 5 = Open a new tab

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RestoreOnStartup
  - GP name: Action to take on startup
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: RestoreOnStartup
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000004
```


  #### Mac information and settings
  - Preference Key Name: RestoreOnStartup
  - Example value:
``` xml
<integer>4</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RestoreOnStartupURLs
  #### Sites to open when the browser starts
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the [RestoreOnStartup](#restoreonstartup) policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RestoreOnStartupURLs
  - GP name: Sites to open when the browser starts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended\RestoreOnStartupURLs
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = https://contoso.com
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\2 = https://www.fabrikam.com

```


  #### Mac information and settings
  - Preference Key Name: RestoreOnStartupURLs
  - Example value:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ShowHomeButton
  #### Show Home button on toolbar
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Shows the Home button on Microsoft Edge's toolbar.

Enable this policy to always show the Home button. Disable it to never show the button.

If you don't configure the policy, users can choose whether to show the home button.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ShowHomeButton
  - GP name: Show Home button on toolbar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ShowHomeButton
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ShowHomeButton
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ## Additional policies

  [Back to top](#microsoft-edge---policies)

  ### AddressBarMicrosoftSearchInBingProviderEnabled
  #### Enable Microsoft Search in Bing suggestions in the address bar
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  Enables the display of relevant Microsoft Search in Bing suggestions in the address bar's suggestion list when the user types a search string in the address bar. If you enable or don't configure this policy, users can see internal results powered by Microsoft Search in Bing in the Microsoft Edge address bar suggestion list. To see the Microsoft Search in Bing results, the user must be signed into Microsoft Edge with their Azure AD account for that organization.
If you disable this policy, users can't see internal results in the Microsoft Edge address bar suggestion list.
If you have enabled the set of policies which forces a default search provider ([DefaultSearchProviderEnabled](#defaultsearchproviderenabled), [DefaultSearchProviderName](#defaultsearchprovidername) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)), and the search provider specified is not Bing, then this policy is not applicable and there will be no Microsoft Search in Bing suggestions in the address bar's suggestion list.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AddressBarMicrosoftSearchInBingProviderEnabled
  - GP name: Enable Microsoft Search in Bing suggestions in the address bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AddressBarMicrosoftSearchInBingProviderEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AddressBarMicrosoftSearchInBingProviderEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AdsSettingForIntrusiveAdsSites
  #### Ads setting for sites with intrusive ads
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Controls whether ads are blocked on sites with intrusive ads. You can set this policy to one of the following options:

* 1 = Allow ads on all sites.

* 2 = Block ads on sites with intrusive ads (Default value).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AdsSettingForIntrusiveAdsSites
  - GP name: Ads setting for sites with intrusive ads
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AdsSettingForIntrusiveAdsSites
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AdsSettingForIntrusiveAdsSites
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowDeletingBrowserHistory
  #### Enable deleting browser and download history
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables deleting browser history and download history and prevents users from changing this setting.

Note that even with this policy is disabled, the browsing and download history aren't guaranteed to be retained: users can edit or delete the history database files directly, and the browser itself may remove (based on expiration period) or archive any or all history items at any time.

If you enable this policy or don't configure it, users can delete the browsing and download history.

If you disable this policy, users can't delete browsing and download history.

If you enable this policy, don't enable the [ClearBrowsingDataOnExit](#clearbrowsingdataonexit) policy, because they both deal with deleting data. If you enable both, the [ClearBrowsingDataOnExit](#clearbrowsingdataonexit) policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how this policy is configured.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowDeletingBrowserHistory
  - GP name: Enable deleting browser and download history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowDeletingBrowserHistory
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AllowDeletingBrowserHistory
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowFileSelectionDialogs
  #### Allow file selection dialogs
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allow access to local files by letting Microsoft Edge display file selection dialogs.

If you enable or don't configure this policy, users can open file selection dialogs as normal.

If you disable this policy, whenever the user performs an action that triggers a file selection dialog (like importing favorites, uploading files, or saving links), a message is displayed instead, and the user is assumed to have clicked Cancel on the file selection dialog.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowFileSelectionDialogs
  - GP name: Allow file selection dialogs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowFileSelectionDialogs
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AllowFileSelectionDialogs
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowPopupsDuringPageUnload
  #### Allows a page to show popups during its unloading
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  This policy allows an admin to specify that a page can show popups during its unloading.

When the policy is set to enabled, pages are allowed to show popups while they're being unloaded.

When the policy is set to disabled or unset, pages aren't allowed to show popups while they're being unloaded. This is as per the spec: (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

This policy will be removed in the future.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowPopupsDuringPageUnload
  - GP name: Allows a page to show popups during its unloading
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowPopupsDuringPageUnload
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AllowPopupsDuringPageUnload
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowSurfGame
  #### Allow surf game
  
  #### Supported versions:
  - On Windows and macOS since 82 or later

  #### Description
  If you disable this policy, users won't be able to play the surf game when the device is offline or if the user navigates to edge://surf.

If you enable or don't configure this policy, users can play the surf game.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowSurfGame
  - GP name: Allow surf game
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowSurfGame
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AllowSurfGame
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowSyncXHRInPageDismissal
  #### Allow pages to send synchronous XHR requests during page dismissal
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  This policy lets you specify that a page can send synchronous XHR requests during page dismissal.

If you enable this policy, pages can send synchronous XHR requests during page dismissal.

If you disable this policy or don't configure this policy, pages aren't allowed to send synchronous XHR requests during page dismissal.

This policy is temporary and will be removed in a future release.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowSyncXHRInPageDismissal
  - GP name: Allow pages to send synchronous XHR requests during page dismissal
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AllowSyncXHRInPageDismissal
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AllowSyncXHRInPageDismissal
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AllowTokenBindingForUrls
  #### Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with.
  
  #### Supported versions:
  - On Windows since 83 or later

  #### Description
  Configure the list of URL patterns for sites that the browser will attempt to perform the Token Binding protocol with.
For the domains on this list, the browser will send the Token Binding ClientHello in the TLS handshake (See https://tools.ietf.org/html/rfc8472).
If the server responds with a valid ServerHello response, the browser will create and send Token Binding messages on subsequent https requests. See https://tools.ietf.org/html/rfc8471 for more info.

If this list is empty, Token Binding will be disabled.

This policy is only available on Windows 10 devices with Virtual Secure Mode capability.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowTokenBindingForUrls
  - GP name: Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with.
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AllowTokenBindingForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTokenBindingForUrls\1 = mydomain.com
SOFTWARE\Policies\Microsoft\Edge\AllowTokenBindingForUrls\2 = [*.]mydomain2.com
SOFTWARE\Policies\Microsoft\Edge\AllowTokenBindingForUrls\3 = [*.].mydomain2.com

```


  

  [Back to top](#microsoft-edge---policies)

  ### AllowTrackingForUrls
  #### Configure tracking prevention exceptions for specific sites
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Configure the list of URL patterns that are excluded from tracking prevention.

If you configure this policy, the list of configured URL patterns is excluded from tracking prevention.

If you don't configure this policy, the global default value from the "Block tracking of users' web-browsing activity" policy (if set) or the user's personal configuration is used for all sites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AllowTrackingForUrls
  - GP name: Configure tracking prevention exceptions for specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\2 = [*.]contoso.edu

```


  #### Mac information and settings
  - Preference Key Name: AllowTrackingForUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AlternateErrorPagesEnabled
  #### Suggest similar pages when a webpage can’t be found
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Allow Microsoft Edge to issue a connection to a web service to generate URL and search suggestions for connectivity issues such as DNS errors.

If you enable this policy, a web service is used to generate url and search suggestions for network errors.

If you disable this policy, no calls to the web service are made and a standard error page is shown.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Suggest similar pages when a webpage can’t be found** toggle, which the user can switch on or off. Note that if you have enable this policy (AlternateErrorPagesEnabled), the Suggest similar pages when a webpage can’t be found setting is turned on, but the user can't change the setting by using the toggle. If you disable this policy, the Suggest similar pages when a webpage can’t be found setting is turned off, and the user can't change the setting by using the toggle.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AlternateErrorPagesEnabled
  - GP name: Suggest similar pages when a webpage can’t be found
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: AlternateErrorPagesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AlternateErrorPagesEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AlwaysOpenPdfExternally
  #### Always open PDF files externally
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables the internal PDF viewer in Microsoft Edge.

If you enable this policy Microsoft Edge treats PDF files as downloads and lets users open them with the default application.

If you don't configure this policy or disable it, Microsoft Edge will open PDF files (unless the user disables it).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AlwaysOpenPdfExternally
  - GP name: Always open PDF files externally
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AlwaysOpenPdfExternally
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AlwaysOpenPdfExternally
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AmbientAuthenticationInPrivateModesEnabled
  #### Enable Ambient Authentication for InPrivate and Guest profiles
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  Configure this policy to allow/disallow ambient authentication for InPrivate and Guest profiles in Microsoft Edge.

Ambient Authentication is http authentication with default credentials when explicit credentials aren't provided via NTLM/Kerberos/Negotiate challenge/response schemes.

If you set the policy to RegularOnly (value 0), it allows ambient authentication for Regular sessions only. InPrivate and Guest sessions won't be allowed to ambiently authenticate.

If you set the policy to InPrivateAndRegular (value 1), it allows ambient authentication for InPrivate and Regular sessions. Guest sessions won't be allowed to ambiently authenticate.

If you set the policy to GuestAndRegular (value 2), it allows ambient authentication for Guest and Regular sessions. InPrivate sessions won't be allowed to ambiently authenticate

If you set the policy to All (value 3), it allows ambient authentication for all sessions.

Note that ambient authentication is always allowed on regular profiles.

In Microsoft Edge version 81 and later, if the policy is left not set, ambient authentication will be enabled in regular sessions only.

* 0 = Enable ambient authentication in regular sessions only

* 1 = Enable ambient authentication in InPrivate and regular sessions

* 2 = Enable ambient authentication in guest and regular sessions

* 3 = Enable ambient authentication in regular, InPrivate and guest sessions

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AmbientAuthenticationInPrivateModesEnabled
  - GP name: Enable Ambient Authentication for InPrivate and Guest profiles
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AmbientAuthenticationInPrivateModesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AmbientAuthenticationInPrivateModesEnabled
  - Example value:
``` xml
<integer>0</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ApplicationLocaleValue
  #### Set application locale
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  Configures the application locale in Microsoft Edge and prevents users from changing the locale.

If you enable this policy, Microsoft Edge uses the specified locale. If the configured locale isn't supported, 'en-US' is used instead.

If you disable or don't configure this setting, Microsoft Edge uses either the user-specified preferred locale (if configured) or the fallback locale 'en-US'.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ApplicationLocaleValue
  - GP name: Set application locale
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ApplicationLocaleValue
  - Value Type: REG_SZ
  ##### Example value:
```
en
```


  

  [Back to top](#microsoft-edge---policies)

  ### AudioCaptureAllowed
  #### Allow or block audio capture
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

This policy affects all types of audio inputs, not only the built-in microphone.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AudioCaptureAllowed
  - GP name: Allow or block audio capture
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AudioCaptureAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AudioCaptureAllowed
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AudioCaptureAllowedUrls
  #### Sites that can access audio capture devices without requesting permission
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify websites, based on URL patterns, that can use audio capture devices without asking the user for permission. Patterns in this list are matched against the security origin of the requesting URL. If they match, the site is automatically granted access to audio capture devices.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AudioCaptureAllowedUrls
  - GP name: Sites that can access audio capture devices without requesting permission
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = https://www.contoso.com/
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\2 = https://[*.]contoso.edu/

```


  #### Mac information and settings
  - Preference Key Name: AudioCaptureAllowedUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AudioSandboxEnabled
  #### Allow the audio sandbox to run
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  This policy controls the audio process sandbox.

If you enable this policy, the audio process will run sandboxed.

If you disable this policy, the audio process will run unsandboxed and the WebRTC audio-processing module will run in the renderer process.
This leaves users open to security risks related to running the audio subsystem unsandboxed.

If you don't configure this policy, the default configuration for the audio sandbox will be used, which might differ based on the platform.

This policy is intended to give enterprises flexibility to disable the audio sandbox if they use security software setups that interfere with the sandbox.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AudioSandboxEnabled
  - GP name: Allow the audio sandbox to run
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AudioSandboxEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AudioSandboxEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AutoImportAtFirstRun
  #### Automatically import another browser's data and settings at first run
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable this policy, Microsoft Edge automatically and silently imports all supported datatypes and settings from the specified browser. This also forces Microsoft Edge to skip the import section of the first-run experience.

Note: This policy currently supports importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (on macOS) browsers.

The browser data from Microsoft Edge Legacy will always be silently migrated at the first run, irrespective of the value of this policy. You can use the following values for this policy:

* 0 = Automatically imports all supported datatypes and settings from the default browser

* 1 = Automatically imports all supported datatypes and settings from Internet Explorer

* 2 = Automatically imports all supported datatypes and settings from Google Chrome

* 3 = Automatically imports all supported datatypes and settings from Safari

* 4 = Disables automatic import, and the import section of the first-run experience is skipped

If this policy is set to the default value (0), then depending on which browser is set as the default browser on the managed device, the corresponding datatypes will be imported into the new Microsoft Edge during the First Run Experience.

If the browser specified as the value of this policy is not present in the managed device, Microsoft Edge will simply skip the import without any notification to the user.

If you set this policy to 'DisabledAutoImport' (4), the import section of the first-run experience is skipped entirely and Microsoft Edge doesn't import browser data and settings automatically.

If this policy is set to the value of Internet Explorer (1), the following datatypes will be imported from the Internet Explorer instance on the managed device:
1. Favorites or bookmarks
2. Saved passwords
3. Search engines
4. Browsing history
5. Home page

If this policy is set to the value of Google Chrome (2), the following datatypes will be imported from the Google Chrome instance on the managed device:
1. Favorites
2. Saved passwords
3. Addresses and more
4. Payment info
5. Browsing history
6. Settings
7. Pinned and Open tabs
8. Extensions
9. Cookies

Note: For a more detailed look at everything that is imported from Google Chrome during the new First Run Experience, please see [https://go.microsoft.com/fwlink/?linkid=2120835](https://go.microsoft.com/fwlink/?linkid=2120835)

If this policy is set to the value of Safari (3), the following datatypes will be imported from the Safari instance on the managed device:
1. Favorites or bookmarks
2. Browsing history

If you want to restrict specific datatypes from getting imported on the managed devices, you can use this policy with other policies such as [ImportAutofillFormData](#importautofillformdata), [ImportBrowserSettings](#importbrowsersettings), [ImportFavorites](#importfavorites), and etc.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AutoImportAtFirstRun
  - GP name: Automatically import another browser's data and settings at first run
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AutoImportAtFirstRun
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: AutoImportAtFirstRun
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AutofillAddressEnabled
  #### Enable AutoFill for addresses
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables the AutoFill feature and allows users to auto-complete address information in web forms using previously stored information.

If you disable this policy, AutoFill never suggests or fills in address information, nor does it save additional address information that the user might submit while browsing the web.

If you enable this policy or don't configure it, users can control AutoFill for addresses in the user interface.

Note that if you disable this policy you also stop all activity for all web forms, except payment and password forms. No further entries are saved, and Microsoft Edge won't suggest or AutoFill any previous entries.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AutofillAddressEnabled
  - GP name: Enable AutoFill for addresses
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: AutofillAddressEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AutofillAddressEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AutofillCreditCardEnabled
  #### Enable AutoFill for credit cards
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables Microsoft Edge's AutoFill feature and lets users auto complete credit card information in web forms using previously stored information.

If you disable this policy, AutoFill never suggests or fills credit card information, nor will it save additional credit card information that users might submit while browsing the web.

If you enable this policy or don't configure it, users can control AutoFill for credit cards.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AutofillCreditCardEnabled
  - GP name: Enable AutoFill for credit cards
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: AutofillCreditCardEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: AutofillCreditCardEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### AutoplayAllowed
  #### Allow media autoplay for websites
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  This policy sets the media autoplay policy for websites.

The default setting, "Not configured" respects the current media autoplay settings and lets users configure their autoplay settings.

Setting to "Enabled" sets media autoplay to "Allow".  All websites are allowed to autoplay media. Users can’t override this policy.

Setting to "Disabled" sets media autoplay to "Block".  No websites are allowed to autoplay media. Users can’t override this policy.

A tab will need to be closed and re-opened for this policy to take effect.


  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: AutoplayAllowed
  - GP name: Allow media autoplay for websites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: AutoplayAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: AutoplayAllowed
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BackgroundModeEnabled
  #### Continue running background apps after Microsoft Edge closes
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  Allows Microsoft Edge processes to start at OS sign-in and keep running after the last browser window is closed. In this scenario, background apps and the current browsing session remain active, including any session cookies. An open background process displays an icon in the system tray and can always be closed from there.

If you enable this policy, background mode is turned on.

If you disable this policy, background mode is turned off.

If you don't configure this policy, background mode is initially turned off, and the user can configure its behavior in edge://settings/system.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BackgroundModeEnabled
  - GP name: Continue running background apps after Microsoft Edge closes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: BackgroundModeEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### BackgroundTemplateListUpdatesEnabled
  #### Enables background updates to the list of available templates for Collections and other features that use templates
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Lets you enable or disable background updates to the list of available templates for Collections and other features that use templates.  Templates are used to extract rich metadata from a webpage when the page is saved to a collection.

If you enable this setting or the setting is unconfigured, the list of available templates will be downloaded in the background from a Microsoft service every 24 hours.

If you disable this setting the list of available templates will be downloaded on demand. This type of download might result in small performance penalties for Collections and other features.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BackgroundTemplateListUpdatesEnabled
  - GP name: Enables background updates to the list of available templates for Collections and other features that use templates
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BackgroundTemplateListUpdatesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: BackgroundTemplateListUpdatesEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BlockThirdPartyCookies
  #### Block third party cookies
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Block web page elements that aren't from the domain that's in the address bar from setting cookies.

If you enable this policy, web page elements that are not from the domain that is in the address bar can't set cookies

If you disable this policy, web page elements from domains other than in the address bar can set cookies.

If you don't configure this policy, third-party cookies are enabled but users can change this setting.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BlockThirdPartyCookies
  - GP name: Block third party cookies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: BlockThirdPartyCookies
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: BlockThirdPartyCookies
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BrowserAddProfileEnabled
  #### Enable profile creation from the Identity flyout menu or the Settings page
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to create new profiles, using the **Add profile** option.
If you enable this policy or don't configure it, Microsoft Edge allows users to use **Add profile** on the Identity flyout menu or the Settings page to create new profiles.

If you disable this policy, users cannot add new profiles from the Identity flyout menu or the Settings page.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BrowserAddProfileEnabled
  - GP name: Enable profile creation from the Identity flyout menu or the Settings page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BrowserAddProfileEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: BrowserAddProfileEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BrowserGuestModeEnabled
  #### Enable guest mode
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enable the option to allow the use of guest profiles in Microsoft Edge. In a guest profile, the browser doesn't import browsing data from existing profiles, and it deletes browsing data when all guest profiles are closed.

If you enable this policy or don't configure it, Microsoft Edge lets users browse in guest profiles.

If you disable this policy, Microsoft Edge doesn't let users browse in guest profiles.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BrowserGuestModeEnabled
  - GP name: Enable guest mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BrowserGuestModeEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: BrowserGuestModeEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BrowserNetworkTimeQueriesEnabled
  #### Allow queries to a Browser Network Time service
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Prevents Microsoft Edge from occasionally sending queries to a browser network time service to retrieve an accurate timestamp.

If you disable this policy, Microsoft Edge will stop sending queries to a browser network time service.

If you enable this policy or don't configure it, Microsoft Edge will occasionally send queries to a browser network time service.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BrowserNetworkTimeQueriesEnabled
  - GP name: Allow queries to a Browser Network Time service
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BrowserNetworkTimeQueriesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: BrowserNetworkTimeQueriesEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BrowserSignin
  #### Browser sign-in settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the [SyncDisabled](#syncdisabled) policy instead.

If you set this policy to 'Disable browser sign-in', make sure that you also set the [NonRemovableProfileEnabled](#nonremovableprofileenabled) policy to disabled because [NonRemovableProfileEnabled](#nonremovableprofileenabled) disables the creation of an automatically signed in browser profile. If both policies are set, Microsoft Edge will use the 'Disable browser sign-in' policy and behave as if [NonRemovableProfileEnabled](#nonremovableprofileenabled) is set to disabled.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing into the browser doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature.

If you set this policy to 'Force browser sign-in' (2) users must sign into a profile to use the browser. By default, this will allow the user to choose whether they want to sync to their account, unless sync is disabled by the domain admin or with the [SyncDisabled](#syncdisabled) policy. The default value of [BrowserGuestModeEnabled](#browserguestmodeenabled) policy is set to false.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BrowserSignin
  - GP name: Browser sign-in settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BrowserSignin
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: BrowserSignin
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### BuiltInDnsClientEnabled
  #### Use built-in DNS client
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Controls whether to use the built-in DNS client.

This does not affect which DNS servers are used; just the software stack which is used to communicate with them. For example if the operating system is configured to use an enterprise DNS server, that same server would be used by the built-in DNS client. It is however possible that the built-in DNS client will address servers in different ways by using more modern DNS-related protocols such as DNS-over-TLS.

If you enable this policy, the built-in DNS client is used, if it's available.

If you disable this policy, the client is never used.

If you don't configure this policy, the built-in DNS client is enabled by default on MacOS, and users can change whether to use the built-in DNS client by editing edge://flags or by specifying a command-line flag.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: BuiltInDnsClientEnabled
  - GP name: Use built-in DNS client
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: BuiltInDnsClientEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: BuiltInDnsClientEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables enforcement of Certificate Transparency requirements for a list of subjectPublicKeyInfo hashes.

This policy lets you disable Certificate Transparency disclosure requirements for certificate chains that contain certificates with one of the specified subjectPublicKeyInfo hashes. This allows certificates that would otherwise be untrusted because they were not properly publicly disclosed to still be used for Enterprise hosts.

To disable Certificate Transparency enforcement when this policy is set, one of the following sets of conditions must be met:
1. The hash is of the server certificate's subjectPublicKeyInfo.
2. The hash is of a subjectPublicKeyInfo that appears in a CA certificate in the certificate chain, that CA certificate is constrained via the X.509v3 nameConstraints extension, one or more directoryName nameConstraints are present in the permittedSubtrees, and the directoryName contains an organizationName attribute.
3. The hash is of a subjectPublicKeyInfo that appears in a CA certificate in the certificate chain, the CA certificate has one or more organizationName attributes in the certificate Subject, and the server's certificate contains the same number of organizationName attributes, in the same order, and with byte-for-byte identical values.

A subjectPublicKeyInfo hash is specified by concatenating the hash algorithm name, the "/" character, and the Base64 encoding of that hash algorithm applied to the DER-encoded subjectPublicKeyInfo of the specified certificate. This Base64 encoding is the same format as an SPKI Fingerprint, as defined in RFC 7469, Section 2.4. Unrecognized hash algorithms are ignored. The only supported hash algorithm at this time is "sha256".

If you disable this policy or don't configure it, any certificate that's required to be disclosed via Certificate Transparency will be treated as untrusted if it's not disclosed according to the Certificate Transparency policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForCas
  - GP name: Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = sha256/AAAAAAAAAAAAAAAAAAAAAA==
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\2 = sha256//////////////////////w==

```


  #### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForCas
  - Example value:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Disable Certificate Transparency enforcement for a list of legacy certificate authorities
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables enforcing Certificate Transparency requirements for a list of legacy certificate authorities (Cas).

This policy lets you disable Certificate Transparency disclosure requirements for certificate chains that contain certificates with one of the specified subjectPublicKeyInfo hashes. This allows certificates that would otherwise be untrusted because they were not properly publicly disclosed, continue to be used for enterprise hosts.

In order for Certificate Transparency enforcement to be disabled, you must set the hash to a subjectPublicKeyInfo appearing in a CA certificate that is recognized as a legacy certificate authority (CA). A legacy CA is a CA that has been publicly trusted by default by one or more operating systems supported by Microsoft Edge.

You specify a subjectPublicKeyInfo hash by concatenating the hash algorithm name, the "/" character, and the Base64 encoding of that hash algorithm applied to the DER-encoded subjectPublicKeyInfo of the specified certificate. This Base64 encoding is the same format as an SPKI Fingerprint, as defined in RFC 7469, Section 2.4. Unrecognized hash algorithms are ignored. The only supported hash algorithm at this time is "sha256".

If you don't configure this policy, any certificate that's required to be disclosed via Certificate Transparency will be treated as untrusted if it isn't disclosed according to the Certificate Transparency policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForLegacyCas
  - GP name: Disable Certificate Transparency enforcement for a list of legacy certificate authorities
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = sha256/AAAAAAAAAAAAAAAAAAAAAA==
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\2 = sha256//////////////////////w==

```


  #### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Example value:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Disable Certificate Transparency enforcement for specific URLs
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables enforcing Certificate Transparency requirements for the listed URLs.

This policy lets you not disclose certificates for the hostnames in the specified URLs via Certificate Transparency. This lets you use certificates that would otherwise be untrusted, because they weren't properly publicly disclosed, but it makes it harder to detect mis-issued certificates for those hosts.

Form your URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Because certificates are valid for a given hostname, independent of the scheme, port, or path, only the hostname part of the URL is considered. Wildcard hosts are not supported.

If you don't configure this policy, any certificate that should be disclosed via Certificate Transparency is treated as untrusted if it's not disclosed.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForUrls
  - GP name: Disable Certificate Transparency enforcement for specific URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = contoso.com
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\2 = .contoso.com

```


  #### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForUrls
  - Example value:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ClearBrowsingDataOnExit
  #### Clear browsing data when Microsoft Edge closes
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Microsoft Edge doesn't clear the browsing data by default when it closes. Browsing data includes information entered in forms, passwords, and even the websites visited.

If you enable this policy, all browsing data is deleted each time Microsoft Edge closes. Note that if you enable this policy, it takes precedence over how you configured [DefaultCookiesSetting](#defaultcookiessetting)

If you disable or don't configure this policy, users can configure the Clear browsing data option in Settings.

If you enable this policy, don't configure the [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) or the [ClearCachedImagesAndFilesOnExit](#clearcachedimagesandfilesonexit) policy, because they all deal with deleting browsing data. If you configure the preceding policies and this policy, all browsing data is deleted when Microsoft Edge closes, regardless of how you configured [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) or [ClearCachedImagesAndFilesOnExit](#clearcachedimagesandfilesonexit).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ClearBrowsingDataOnExit
  - GP name: Clear browsing data when Microsoft Edge closes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ClearBrowsingDataOnExit
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ClearBrowsingDataOnExit
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ClearCachedImagesAndFilesOnExit
  #### Clear cached images and files when Microsoft Edge closes
  
  #### Supported versions:
  - On Windows and macOS since 82 or later

  #### Description
  Microsoft Edge doesn't clear cached images and files by default when it closes.

If you enable this policy, cached images and files will be deleted each time Microsoft Edge closes.

If you disable this policy, users cannot configure the cached images and files option in edge://settings/clearBrowsingDataOnClose.

If you don't configure this policy, users can choose whether cached images and files are cleared on exit.

If you disable this policy, don't enable the [ClearBrowsingDataOnExit](#clearbrowsingdataonexit) policy, because they both deal with deleting data. If you configure both, the [ClearBrowsingDataOnExit](#clearbrowsingdataonexit) policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how you configured [ClearCachedImagesAndFilesOnExit](#clearcachedimagesandfilesonexit).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ClearCachedImagesAndFilesOnExit
  - GP name: Clear cached images and files when Microsoft Edge closes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ClearCachedImagesAndFilesOnExit
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ClearCachedImagesAndFilesOnExit
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ClickOnceEnabled
  #### Allow users to open files using the ClickOnce protocol
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  Allow users to open files using the ClickOnce protocol. The ClickOnce protocol allows websites to request that the browser open files from a specific URL using the ClickOnce file handler on the user's computer or device.

If you enable this policy, users can open files using the ClickOnce protocol. This policy overrides the user's ClickOnce setting in the edge://flags/ page.

If you disable this policy, users can't open files using the ClickOnce protocol. Instead, the file will be saved to the file system using the browser. This policy overrides the user's ClickOnce setting in the edge://flags/ page.

If you don't configure this policy, users can't open files using the ClickOnce protocol. Users have the option to enable the use of the ClickOnce protocol with the edge://flags/ page.

Disabling ClickOnce may prevent ClickOnce applications (.application files) from launching properly.

For more information about ClickOnce, see [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) and [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ClickOnceEnabled
  - GP name: Allow users to open files using the ClickOnce protocol
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ClickOnceEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Enable security warnings for command-line flags
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  If disabled, this policy prevents security warnings from appearing when Microsoft Edge is launched with potentially dangerous command-line flags.

If enabled or unset, security warnings are displayed when these command-line flags are used to launch Microsoft Edge.

For example, the --disable-gpu-sandbox flag generates this warning:  You're using an unsupported command-line flag: --disable-gpu-sandbox. This poses stability and security risks.

On Windows, this policy is only available on instances that are joined to a Microsoft Active Directory domain, or Windows 10 Pro (or Enterprise) instances that are enrolled for device management.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CommandLineFlagSecurityWarningsEnabled
  - GP name: Enable security warnings for command-line flags
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: CommandLineFlagSecurityWarningsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: CommandLineFlagSecurityWarningsEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ComponentUpdatesEnabled
  #### Enable component updates in Microsoft Edge
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable or don't configure this policy, component updates are enabled in Microsoft Edge.

If you disable this policy or set it to false, component updates are disabled for all components in Microsoft Edge.

However, some components are exempt from this policy. This includes any component that doesn't contain executable code, that doesn't significantly alter the behavior of the browser, or that's critical for security. That is, updates that are deemed "critical for security" are still applied even if you disable this policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ComponentUpdatesEnabled
  - GP name: Enable component updates in Microsoft Edge
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ComponentUpdatesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ComponentUpdatesEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ConfigureDoNotTrack
  #### Configure Do Not Track
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify whether to send Do Not Track requests to websites that ask for tracking info. Do Not Track requests let the websites you visit know that you don't want your browsing activity to be tracked. By default, Microsoft Edge doesn't send Do Not Track requests, but users can turn on this feature to send them.

If you enable this policy, Do Not Track requests are always sent to websites asking for tracking info.

If you disable this policy, requests are never sent.

If you don't configure this policy, users can choose whether to send these requests.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ConfigureDoNotTrack
  - GP name: Configure Do Not Track
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ConfigureDoNotTrack
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ConfigureDoNotTrack
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ConfigureOnPremisesAccountAutoSignIn
  #### Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account
  
  #### Supported versions:
  - On Windows since 81 or later

  #### Description
  Enable the use of Active Directory accounts for automatic sign in if your users' machines are Domain Joined and your environment is not hybrid joined. If you want users automatically signed in with their Azure Active Directory accounts instead, please Azure AD join (See [https://go.microsoft.com/fwlink/?linkid=2118197](https://go.microsoft.com/fwlink/?linkid=2118197) for more information) or hybrid join (See [https://go.microsoft.com/fwlink/?linkid=2118365](https://go.microsoft.com/fwlink/?linkid=2118365) for more information) your environment.

If you have configured the [BrowserSignin](#browsersignin) policy to disabled, this policy will not take any effect.

If you enable this policy and set it to "Sign in and make domain account non-removable", Microsoft Edge will automatically sign in users that are on domain joined machines using their Active Directory accounts.

If you set this policy to "Disabled" or don't set it, Microsoft Edge will not automatically sign in users that are on domain joined machines with Active Directory accounts.

* 0 = Disabled

* 1 = Sign in and make domain account non-removable

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ConfigureOnPremisesAccountAutoSignIn
  - GP name: Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ConfigureOnPremisesAccountAutoSignIn
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### ConfigureOnlineTextToSpeech
  #### Configure Online Text To Speech
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether the browser can leverage Online Text to Speech voice fonts, part of Azure Cognitive Services. These voice fonts are higher quality than the pre-installed system voice fonts.

If you enable or don't configure this policy, web-based applications that use the SpeechSynthesis API can use Online Text to Speech voice fonts.

If you disable this policy, the voice fonts aren't available.

Read more about this feature here:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Cognitive Services: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ConfigureOnlineTextToSpeech
  - GP name: Configure Online Text To Speech
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ConfigureOnlineTextToSpeech
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ConfigureOnlineTextToSpeech
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ConfigureShare
  #### Configure the Share experience
  
  #### Supported versions:
  - On Windows since 82 or later

  #### Description
  If you set this policy to 'ShareAllowed' (0, the default), users will be able to access the Windows 10 Share experience from the Settings and More Menu in Microsoft Edge to share with other apps on the system.

If you set this policy to 'ShareDisallowed' (1), users won't be able to access the Windows 10 Share experience. If the Share button is on the toolbar, it will also be hidden.

* 0 = Allow using the Share experience

* 1 = Don't allow using the Share experience


  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ConfigureShare
  - GP name: Configure the Share experience
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ConfigureShare
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### CustomHelpLink
  #### Specify custom help link
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Specify a link for the Help menu or the F1 key.

If you enable this policy, an admin can specify a link for the Help menu or the F1 key.

If you disable or don't configure this policy, the default link for the Help menu or the F1 key is used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: CustomHelpLink
  - GP name: Specify custom help link
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: CustomHelpLink
  - Value Type: REG_SZ
  ##### Example value:
```
https://go.microsoft.com/fwlink/?linkid=2080734
```


  #### Mac information and settings
  - Preference Key Name: CustomHelpLink
  - Example value:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DNSInterceptionChecksEnabled
  #### DNS interception checks enabled
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  This policy configures a local switch that can be used to disable DNS interception checks. These checks attempt to discover whether the browser is behind a proxy that redirects unknown host names.

This detection might not be necessary in an enterprise environment where the network configuration is known. It can be disabled to avoid additional DNS and HTTP traffic on start-up and each DNS configuration change.

If you enable or don’t set this policy, the DNS interception checks are performed.

If you disable this policy, DNS interception checks aren’t performed.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DNSInterceptionChecksEnabled
  - GP name: DNS interception checks enabled
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DNSInterceptionChecksEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DNSInterceptionChecksEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DefaultBrowserSettingEnabled
  #### Set Microsoft Edge as default browser
  
  #### Supported versions:
  - On Windows 7 and macOS since 77 or later

  #### Description
  Configures the default browser checks in Microsoft Edge and prevents users from changing them.

If you enable this policy, Microsoft Edge always checks on startup whether it is the default browser and automatically registers itself, if possible.

If you disable this policy, Microsoft Edge never checks and disables user controls for setting this option.

If you don't configure this policy, Microsoft Edge lets the user control whether it's the default browser and whether to show user notifications when it isn't.

Note for Windows administrators: This policy only works for PCs running Windows 7. For later versions of Windows, you have to deploy a "default application associations" file that makes Microsoft Edge the handler for the https and http protocols (and, optionally, the ftp protocol and file formats such as .html, .htm, .pdf, .svg, .webp). See [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932) for more information.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DefaultBrowserSettingEnabled
  - GP name: Set Microsoft Edge as default browser
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DefaultBrowserSettingEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DefaultBrowserSettingEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DeleteDataOnMigration
  #### Delete old browser data on migration
  
  #### Supported versions:
  - On Windows since 82 or later

  #### Description
  This policy determines whether user browsing data from Microsoft Edge Legacy will be deleted after migrating to the Microsoft Edge version 81 or later.

If you set this policy to "Enabled", all browsing data from Microsoft Edge Legacy after migrating to the Microsoft Edge version 81 or later will be deleted. This policy must be set before migrating to the Microsoft Edge version 81 or later to have any effect on existing browsing data.

If you set this policy to "Disabled", or the policy is not configured, user browsing data isn't deleted after migrating to the Microsoft Edge version 82 or later.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DeleteDataOnMigration
  - GP name: Delete old browser data on migration
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DeleteDataOnMigration
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### DeveloperToolsAvailability
  #### Control where developer tools can be used
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Control where developer tools can be used.

If you set this policy to 'DeveloperToolsDisallowedForForceInstalledExtensions' (0, the default), users can access the developer tools and the JavaScript console in general, but not in the context of extensions installed by enterprise policy.

If you set this policy to 'DeveloperToolsAllowed' (1), users can access the developer tools and the JavaScript console in all contexts, including extensions installed by enterprise policy.

If you set this policy to 'DeveloperToolsDisallowed' (2), users can't access the developer tools or inspect website elements. Keyboard shortcuts and menu or context menu entries that open the developer tools or the JavaScript Console are disabled.

* 0 = Block the developer tools on extensions installed by enterprise policy, allow in other contexts

* 1 = Allow using the developer tools

* 2 = Don't allow using the developer tools

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DeveloperToolsAvailability
  - GP name: Control where developer tools can be used
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DeveloperToolsAvailability
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DeveloperToolsAvailability
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DirectInvokeEnabled
  #### Allow users to open files using the DirectInvoke protocol
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  Allow users to open files using the DirectInvoke protocol. The DirectInvoke protocol allows websites to request that the browser open files from a specific URL using a specific file handler on the user's computer or device.

If you enable or don't configure this policy, users can open files using the DirectInvoke protocol.

If you disable this policy, users can't open files using the DirectInvoke protocol. Instead, the file will be saved to the file system.

Note: Disabling DirectInvoke may prevent certain Microsoft SharePoint Online features from working as expected.

For more information about DirectInvoke, see [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) and [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DirectInvokeEnabled
  - GP name: Allow users to open files using the DirectInvoke protocol
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DirectInvokeEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### Disable3DAPIs
  #### Disable support for 3D graphics APIs
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: Disable3DAPIs
  - GP name: Disable support for 3D graphics APIs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: Disable3DAPIs
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: Disable3DAPIs
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DisableScreenshots
  #### Disable taking screenshots
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Controls if users can take screenshots of the browser page.

If enabled, user can't take screenshots by using keyboard shortcuts or extension APIs.

If disabled or don't configure this policy, users can take screenshots.

Please note this policy controls screenshots taken from within the browser itself. Even if you enable this policy, users might still be able to take screenshots using some method outside of the browser (like using an operating system feature or another application).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DisableScreenshots
  - GP name: Disable taking screenshots
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DisableScreenshots
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: DisableScreenshots
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DiskCacheDir
  #### Set disk cache directory
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the directory to use to store cached files.

If you enable this policy, Microsoft Edge uses the provided directory regardless of whether the user has specified the '--disk-cache-dir' flag. To avoid data loss or other unexpected errors, don't configure this policy to a volume's root directory or to a directory used for other purposes, because Microsoft Edge manages its contents.

See [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) for a list of variables you can use when specifying directories and paths.

If you don't configure this policy, the default cache directory is used, and users can override that default with the '--disk-cache-dir' command line flag.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DiskCacheDir
  - GP name: Set disk cache directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DiskCacheDir
  - Value Type: REG_SZ
  ##### Example value:
```
${user_home}/Edge_cache
```


  #### Mac information and settings
  - Preference Key Name: DiskCacheDir
  - Example value:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DiskCacheSize
  #### Set disk cache size, in bytes
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the size of the cache, in bytes, used to store files on the disk.

If you enable this policy, Microsoft Edge uses the provided cache size regardless of whether the user has specified the '--disk-cache-size' flag. The value specified in this policy isn't a hard boundary but rather a suggestion to the caching system; any value below a few megabytes is too small and will be rounded up to a reasonable minimum.

If you set the value of this policy to 0, the default cache size is used, and users can't change it.

If you don't configure this policy, the default size is used, but users can override it with the '--disk-cache-size' flag.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DiskCacheSize
  - GP name: Set disk cache size, in bytes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DiskCacheSize
  - Value Type: REG_DWORD
  ##### Example value:
```
0x06400000
```


  #### Mac information and settings
  - Preference Key Name: DiskCacheSize
  - Example value:
``` xml
<integer>104857600</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DnsOverHttpsTemplates
  #### Specify URI template of desired DNS-over-HTTPS resolver
  
  #### Supported versions:
  - On Windows and macOS since 83 or later

  #### Description
  The URI template of the desired DNS-over-HTTPS resolver. To specify multiple DNS-over-HTTPS resolvers, separate the corresponding URI templates with spaces.

If you set the  DnsOverHttpsMode to "secure" then this policy must be set and not be empty.

If you set the DnsOverHttpsMode to "automatic" and this policy is set then the URI templates specified will be used. If you don't set this policy, then hardcoded mappings will be used to attempt to upgrade the user's current DNS resolver to a DoH resolver operated by the same provider.

If the URI template contains a dns variable, requests to the resolver will use GET; otherwise requests will use POST.

Incorrectly formatted templates will be ignored.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DnsOverHttpsTemplates
  - GP name: Specify URI template of desired DNS-over-HTTPS resolver
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: DnsOverHttpsTemplates
  - Value Type: REG_SZ
  ##### Example value:
```
https://dns.example.net/dns-query{?dns}
```


  #### Mac information and settings
  - Preference Key Name: DnsOverHttpsTemplates
  - Example value:
``` xml
<string>https://dns.example.net/dns-query{?dns}</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DownloadDirectory
  #### Set download directory
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the directory to use when downloading files.

If you enable this policy, Microsoft Edge uses the provided directory regardless of whether the user has specified one or chosen to be prompted for download location every time. See [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) for a list of variables that can be used.

If you disable or don't configure this policy, the default download directory is used, and the user can change it.

If you set an invalid path, Microsoft Edge will default to the user's default download directory.

If the folder specified by the path doesn't exist, the download will trigger a prompt that asks the user where they want to save their download.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DownloadDirectory
  - GP name: Set download directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: DownloadDirectory
  - Value Type: REG_SZ
  ##### Example value:
```

      Linux-based OSes (including Mac): /home/${user_name}/Downloads
      Windows: C:\Users\${user_name}\Downloads
```


  #### Mac information and settings
  - Preference Key Name: DownloadDirectory
  - Example value:
``` xml
<string>
      Linux-based OSes (including Mac): /home/${user_name}/Downloads
      Windows: C:\Users\${user_name}\Downloads</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### DownloadRestrictions
  #### Allow download restrictions
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures the type of downloads that Microsoft Edge completely blocks, without letting users override the security decision.

Set 'Block dangerous downloads' (1) to allow all downloads except for those that carry Microsoft Defender SmartScreen warnings.

Set 'Block potentially dangerous downloads' (2) to allow all downloads except for those that carry Microsoft Defender SmartScreen warnings of potentially dangerous downloads.

Set 'Block all downloads' (3) to block all downloads.

If you don't configure this policy or set the 'No special restrictions' (0) option, the downloads go through the usual security restrictions based on Microsoft Defender SmartScreen analysis results.

Note that these restrictions apply to downloads from web page content, as well as the 'download link...' context menu option. These restrictions don't apply to saving or downloading the currently displayed page, nor do they apply to the Save as PDF option from the printing options.

See [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934) for more info on Microsoft Defender SmartScreen.

* 0 = No special restrictions

* 1 = Block dangerous downloads

* 2 = Block potentially dangerous downloads

* 3 = Block all downloads

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: DownloadRestrictions
  - GP name: Allow download restrictions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: DownloadRestrictions
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: DownloadRestrictions
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EdgeCollectionsEnabled
  #### Enable the Collections feature
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Lets you allow users to access the Collections feature, where they can collect, organize, share, and export content more efficiently and with Office integration.

If you enable or don't configure this policy, users can access and use the Collections feature in Microsoft Edge.

If you disable this policy, users can't access and use Collections in Microsoft Edge.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EdgeCollectionsEnabled
  - GP name: Enable the Collections feature
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EdgeCollectionsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: EdgeCollectionsEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EditFavoritesEnabled
  #### Allows users to edit favorites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enable this policy to let users add, remove, and modify favorites. This is the default behavior if you don't configure the policy.

Disable this policy to stop users from adding, removing, or modifying favorites. They can still use existing favorites.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EditFavoritesEnabled
  - GP name: Allows users to edit favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EditFavoritesEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: EditFavoritesEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EnableDeprecatedWebPlatformFeatures
  #### Re-enable deprecated web platform features for a limited time
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify a list of deprecated web platform features to temporarily re-enable.

This policy lets you re-enable deprecated web platform features for a limited time. Features are identified by a string tag.

If you don't configure this policy, if the list is empty, or if a feature doesn't match one of the supported string tags, all deprecated web platform features remain disabled.

While the policy itself is supported on the above platforms, the feature it's enabling might not be available on all of those platforms. Not all deprecated Web Platform features can be re-enabled. Only those explicitly listed below can be re-enabled, and only for a limited period of time, which differs per feature. You can review the intent behind the Web Platform feature changes at https://bit.ly/blinkintents.

The general format of the string tag is [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = Enable ExampleDeprecatedFeature API through 2008/09/02

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnableDeprecatedWebPlatformFeatures
  - GP name: Re-enable deprecated web platform features for a limited time
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\1 = ExampleDeprecatedFeature_EffectiveUntil20080902

```


  #### Mac information and settings
  - Preference Key Name: EnableDeprecatedWebPlatformFeatures
  - Example value:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EnableDomainActionsDownload
  #### Enable Domain Actions Download from Microsoft
  >DEPRECATED: This policy is deprecated. It is currently supported but will become obsolete in a future release.
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Although this policy is used to enable/disable download of the domain actions list, it doesn't always achieve the desired state. The Experimentation and Configuration Service, which handles the download, has its own group policy to configure what is downloaded from the service. To avoid conflicting states, this policy is being deprecated and will be obsolete in milestone 85 onward. Please use the [ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol) policy instead.

In Microsoft Edge, Domain Actions represent a series of compatibility features that help the browser work correctly on the web.

Microsoft keeps a list of actions to take on certain domains for compatibility reasons. For example, the browser may override the User Agent string on a website if that website is broken due to the new User Agent string on Microsoft Edge. Each of these actions is intended to be temporary while Microsoft tries to resolve the issue with the site owner.

When the browser starts up and then periodically afterwards, the browser will contact the Experimentation and Configuration Service that contains the most up to date list of compatibility actions to perform. This list is saved locally after it is first retrieved so that subsequent requests will only update the list if the server's copy has changed.

If you enable this policy, the list of Domain Actions will continue to be downloaded from the Experimentation and Configuration Service.

If you disable this policy, the list of Domain Actions will no longer be downloaded from the Experimentation and Configuration Service.

If you don't configure this policy, the list of Domain Actions will continue to be downloaded from the Experimentation and Configuration Service.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnableDomainActionsDownload
  - GP name: Enable Domain Actions Download from Microsoft %s(deprecated)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EnableDomainActionsDownload
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: EnableDomainActionsDownload
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EnableOnlineRevocationChecks
  #### Enable online OCSP/CRL checks
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Online revocation checks don't provide a significant security benefit and are disabled by default.

If you enable this policy, Microsoft Edge will perform soft-fail, online OCSP/CRL checks. "Soft fail" means that if the revocation server can't be reached, the certificate will be considered valid.

If you disable the policy or don't configure it, Microsoft Edge won't perform online revocation checks.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnableOnlineRevocationChecks
  - GP name: Enable online OCSP/CRL checks
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EnableOnlineRevocationChecks
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: EnableOnlineRevocationChecks
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Allow managed extensions to use the Enterprise Hardware Platform API
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  When this policy is set to enabled, extensions installed by enterprise policy are allowed to use the Enterprise Hardware Platform API.
When this policy is set to disabled or isn't set, no extensions are allowed to use the Enterprise Hardware Platform API.
This policy also applies to component extensions.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: EnterpriseHardwarePlatformAPIEnabled
  - GP name: Allow managed extensions to use the Enterprise Hardware Platform API
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: EnterpriseHardwarePlatformAPIEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: EnterpriseHardwarePlatformAPIEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExperimentationAndConfigurationServiceControl
  #### Control communication with the Experimentation and Configuration Service
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  In Microsoft Edge, the Experimentation and Configuration Service is used to deploy Experimentation and Configuration payload.

Experimentation payload consists of a list of early in development features that Microsoft is enabling for testing and feedback.

Configuration payload consists of a list of settings that Microsoft wants to deploy to Microsoft Edge to optimize user experience. For example, configuration payload may specify how often Microsoft Edge sends requests to the Experimentation and Configuration Service to retrieve the newest payload.

Additionaly, configuration payload may also contain a list of actions to take on certain domains for compatibility reasons. For example, the browser may override the User Agent string on a website if that website is broken due to the new User Agent string on Microsoft Edge. Each of these actions is intended to be temporary while Microsoft tries to resolve the issue with the site owner.

If you set this policy to "Retrieve configurations and experiments" mode, the full payload is downloaded from the Experimentation and Configuration Service. This includes both the experimentation and configuration payloads.

If you set this policy to "Retrieve configurations only" mode, only the configuration payload is delivered.

If you set this policy to "Disable communication with the Experimentation and Configuration Service" mode, the communication with the Experimentation and Configuration Service is stopped completely.

If you don't configure this policy, on a managed device on Stable and Beta channels the behavior is the same as the "Retrieve configurations only" mode.

If you don't configure this policy, on an unmanaged device the behavior is the same as the "Retrieve configurations and experiments" mode.

* 0 = Disable communication with the Experimentation and Configuration Service

* 1 = Retrieve configurations only

* 2 = Retrieve configurations and experiments

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExperimentationAndConfigurationServiceControl
  - GP name: Control communication with the Experimentation and Configuration Service
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ExperimentationAndConfigurationServiceControl
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: ExperimentationAndConfigurationServiceControl
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Show an "Always open" checkbox in external protocol dialog
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  This policy controls whether the "Always allow this site to open links of this type" checkbox is shown on external protocol launch confirmation prompts.

If you set this policy to True, when an external protocol confirmation prompt is shown, the user can select "Always allow" to skip all future confirmation prompts for the protocol on this site.

If you set this policy to False, the "Always allow" checkbox isn't displayed. The user will be prompted for confirmation every time an external protocol is invoked.

If this policy is unset, the checkbox visibility is controlled by the "Enable remembering protocol launch prompting preferences" flag in edge://flags

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - GP name: Show an "Always open" checkbox in external protocol dialog
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### FamilySafetySettingsEnabled
  #### Allow users to configure Family safety
  
  #### Supported versions:
  - On Windows and macOS since 82 or later

  #### Description
  This policy disables and completely hides the Family safety page in Settings. Navigation to edge://settings/familysafety will also be blocked. The Family safety page describes what features are available for family groups and how to join a family group. Learn more about family safety here: ([https://go.microsoft.com/fwlink/?linkid=2098432](https://go.microsoft.com/fwlink/?linkid=2098432)).

If you enable this policy or don't configure it, the Family safety page will be shown.

If you disable this policy, the Family safety page will not be shown.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: FamilySafetySettingsEnabled
  - GP name: Allow users to configure Family safety
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: FamilySafetySettingsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: FamilySafetySettingsEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### FavoritesBarEnabled
  #### Enable favorites bar
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables or disables the favorites bar.

If you enable this policy, users will see the favorites bar.

If you disable this policy, users won't see the favorites bar.

If this policy is not configured, then the user can decide to use the favorites bar or not.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: FavoritesBarEnabled
  - GP name: Enable favorites bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: FavoritesBarEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: FavoritesBarEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceBingSafeSearch
  #### Enforce Bing SafeSearch
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Ensure that queries in Bing web search are done with SafeSearch set to the value specified. Users can't change this setting.

If you configure this policy to "Off", SafeSearch in Bing search falls back to the bing.com value.

If you configure this policy to "Moderate", the moderate setting is used in SafeSearch. The moderate setting filters adult videos and images but not text from search results.

If you configure this policy to "Strict", the strict setting in SafeSearch is used. The strict setting filters adult text, images, and videos.

If you disable this policy or don't configure it, SafeSearch in Bing search isn't enforced, and users can set the value they want on bing.com.

* 0 = Don't configure search restrictions in Bing

* 1 = Configure moderate search restrictions in Bing

* 2 = Configure strict search restrictions in Bing

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceBingSafeSearch
  - GP name: Enforce Bing SafeSearch
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceBingSafeSearch
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ForceBingSafeSearch
  - Example value:
``` xml
<integer>0</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceCertificatePromptsOnMultipleMatches
  #### Configure whether Microsoft Edge should automatically select a certificate when there are multiple certificate matches for a site configured with "AutoSelectCertificateForUrls"
  
  #### Supported versions:
  - On Windows and macOS since 82 or later

  #### Description
  Toggles whether users are prompted to select a certificate if there are multiple certificates available and a site is configured with [AutoSelectCertificateForUrls](#autoselectcertificateforurls). If you don't configure [AutoSelectCertificateForUrls](#autoselectcertificateforurls) for a site, the user will always be prompted to select a certificate.

If you set this policy to True, Microsoft Edge will prompt a user to select a certificate for sites on the list defined in [AutoSelectCertificateForUrls](#autoselectcertificateforurls) if and only if there is more than one certificate.

If you set this policy to False or don't configure it, Microsoft Edge will automatically select a certificate even if there are multiple matches for a certificate. The user will not be prompted to select a certificate for sites on the list defined in [AutoSelectCertificateForUrls](#autoselectcertificateforurls).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceCertificatePromptsOnMultipleMatches
  - GP name: Configure whether Microsoft Edge should automatically select a certificate when there are multiple certificate matches for a site configured with "AutoSelectCertificateForUrls"
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceCertificatePromptsOnMultipleMatches
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ForceCertificatePromptsOnMultipleMatches
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceEphemeralProfiles
  #### Enable use of ephemeral profiles
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Controls whether user profiles are switched to ephemeral mode. An ephemeral profile is created when a session begins, is deleted when the session ends, and is associated with the user's original profile.

If you enable this policy, profiles run in ephemeral mode. This lets users work from their own devices without saving browsing data to those devices. If you enable this policy as an OS policy (by using GPO on Windows, for example), it applies to every profile on the system.

If you disable this policy or don't configure it, users get their regular profiles when they sign in to the browser.

In ephemeral mode, profile data is saved on disk only for the length of the user session. Features like browser history, extensions and their data, web data like cookies, and web databases aren't saved after the browser is closed. This doesn't prevent a user from manually downloading any data to disk, or from saving pages or printing them. If the user has enabled sync, all data is preserved in their sync accounts just like with regular profiles. Users can also use InPrivate browsing in ephemeral mode unless you explicitly disable this.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceEphemeralProfiles
  - GP name: Enable use of ephemeral profiles
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceEphemeralProfiles
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ForceEphemeralProfiles
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceGoogleSafeSearch
  #### Enforce Google SafeSearch
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Forces queries in Google Web Search to be performed with SafeSearch set to active, and prevents users from changing this setting.

If you enable this policy, SafeSearch in Google Search is always active.

If you disable this policy or don't configure it, SafeSearch in Google Search isn't enforced.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceGoogleSafeSearch
  - GP name: Enforce Google SafeSearch
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceGoogleSafeSearch
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ForceGoogleSafeSearch
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceLegacyDefaultReferrerPolicy
  #### Use a default referrer policy of no-referrer-when-downgrade.
  >DEPRECATED: This policy is deprecated. It is currently supported but will become obsolete in a future release.
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  This enterprise policy is for short-term adaptation and will be removed in M82.

Microsoft Edge’s default referrer policy is being strengthened from its current value of no-referrer-when-downgrade to the more secure strict-origin-when-cross-origin through a gradual rollout targeting M80 stable.

Before the rollout, this enterprise policy will have no effect. After the rollout, when this enterprise policy is enabled, Microsoft Edge’s default referrer policy will be set to its pre-M80 value of no-referrer-when-downgrade.

This enterprise policy is disabled by default

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceLegacyDefaultReferrerPolicy
  - GP name: Use a default referrer policy of no-referrer-when-downgrade. %s(deprecated)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceLegacyDefaultReferrerPolicy
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ForceLegacyDefaultReferrerPolicy
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ForceNetworkInProcess
  #### Force networking code to run in the browser process
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  This policy forces networking code to run in the browser process.

This policy is disabled by default. If enabled, users are open to security issues when the networking process is sandboxed.

This policy is intended to give enterprises a chance to migrate to 3rd party software that doesn't depend on hooking networking APIs. Proxy servers are recommended over LSPs and Win32 API patching.

If this policy isn't set, networking code may run out of the browser process depending on field trials of the NetworkService experiment.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceNetworkInProcess
  - GP name: Force networking code to run in the browser process
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceNetworkInProcess
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### ForceYouTubeRestrict
  #### Force minimum YouTube Restricted Mode
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enforces a minimum Restricted Mode on YouTube and prevents users from picking a less restricted mode.

Set to Strict (2) to enforce Strict Restricted Mode on YouTube.

Set to Moderate (1) to enforce the user to only use Moderate Restricted Mode and Strict Restricted Mode on YouTube. They can't disable Restricted Mode.

Set to Off (0) or don't configure this policy to not enforce Restricted Mode on YouTube. External policies such as YouTube policies might still enforce Restricted Mode.

* 0 = Do not enforce Restricted Mode on YouTube

* 1 = Enforce at least Moderate Restricted Mode on YouTube

* 2 = Enforce Strict Restricted Mode for YouTube

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ForceYouTubeRestrict
  - GP name: Force minimum YouTube Restricted Mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ForceYouTubeRestrict
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ForceYouTubeRestrict
  - Example value:
``` xml
<integer>0</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### FullscreenAllowed
  #### Allow full screen mode
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  Set the availability of full screen mode - all Microsoft Edge UI is hidden and only web content is visible.

If you enable this policy or don't configure it, the user, apps, and extensions with appropriate permissions can enter full screen mode.

If you disable this policy, users, apps, and extensions can't enter full screen mode.

Opening Microsoft Edge in kiosk mode using the command line is unavailable when full screen mode is disabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: FullscreenAllowed
  - GP name: Allow full screen mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: FullscreenAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### GloballyScopeHTTPAuthCacheEnabled
  #### Enable globally scoped HTTP auth cache
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  This policy configures a single global per profile cache with HTTP server authentication credentials.

If you disable or don’t set this policy, the browser will use the default behavior of cross-site auth, which as of version 80, will be to scope HTTP server authentication credentials by top-level site. So, if two sites use resources from the same authenticating domain, credentials will need to be provided independently in the context of both sites. Cached proxy credentials will be reused across sites.

If you enable this policy HTTP auth credentials entered in the context of one site will automatically be used in the context of another site.

Enabling this policy leaves sites open to some types of cross-site attacks, and allows users to be tracked across sites even without cookies by adding entries to the HTTP auth cache using credentials embedded in URLs.

This policy is intended to give enterprises depending on the legacy behavior a chance to update their login procedures and will be removed in the future.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: GloballyScopeHTTPAuthCacheEnabled
  - GP name: Enable globally scoped HTTP auth cache
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: GloballyScopeHTTPAuthCacheEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: GloballyScopeHTTPAuthCacheEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### Force direct intranet site navigation instead of searching on single word entries in the Address Bar
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  If you enable this policy, the top auto-suggest result in the address bar suggestion list will navigate to intranet sites if the text entered in the address bar is a single word without punctuation.

Default navigation when typing a single word without punctuation will conduct a navigation to an intranet site matching the entered text.

If you enable this policy, the second auto-suggest result in the address bar suggestion list will conduct a web search exactly as it was entered, provided that this text is a single word without punctuation. The default search provider will be used unless a policy to prevent web search is also enabled.

Two effects of enabling this policy are:

Navigation to sites in response to single word queries that would typically resolve to a history item will no longer happen. Instead, the browser will attempt navigate to internal sites that may not exist in an organization’s intranet. This will result in a 404 error.

Popular, single-word search terms will require manual selection of search suggestions to properly conduct a search.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: GoToIntranetSiteForSingleWordEntryInAddressBar
  - GP name: Force direct intranet site navigation instead of searching on single word entries in the Address Bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### HSTSPolicyBypassList
  #### Configure the list of names that will bypass the HSTS policy check
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Hostnames specified in this list will be exempt from the HSTS policy check that could potentially upgrade requests from "http://" to "https://". Only single-label hostnames are allowed in this policy. Hostnames must be canonicalized. Any IDNs must be converted to their A-label format, and all ASCII letters must be lowercase. This policy only applies to the specific hostnames specified; it doesn't apply to subdomains of the names in the list.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: HSTSPolicyBypassList
  - GP name: Configure the list of names that will bypass the HSTS policy check
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\1 = meet

```


  #### Mac information and settings
  - Preference Key Name: HSTSPolicyBypassList
  - Example value:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### HardwareAccelerationModeEnabled
  #### Use hardware acceleration when available
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify to use hardware acceleration, if it's available. If you enable this policy or don't configure it, hardware acceleration is enabled unless a GPU feature is explicitly blocked.

If you disable this policy, hardware acceleration is disabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: HardwareAccelerationModeEnabled
  - GP name: Use hardware acceleration when available
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: HardwareAccelerationModeEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: HardwareAccelerationModeEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### HideFirstRunExperience
  #### Hide the First-run experience and splash screen
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  If you enable this policy, the First-run experience and the splash screen will not be shown to users when they run Microsoft Edge for the first time.

For the configuration options shown in the First Run Experience, the browser will default to the following:

-On the New Tab Page, the feed type will be set to MSN News and the layout to Inspirational.

-The user will still be automatically signed into Microsoft Edge if the Windows account is of Azure AD or MSA type.

-Sync will not be enabled by default and users will be able to turn on sync from the sync settings.

If you disable or don't configure this policy, the First-run experience and the Splash screen will be shown.

Note: The specific configuration options shown to the user in the First Run Experience, can also be managed by using other specific policies. You can use the HideFirstRunExperience policy in combination with these policies to configure a specific browser experience on your managed devices. Some of these other policies are:

-[AutoImportAtFirstRun](#autoimportatfirstrun)

-[NewTabPageLocation](#newtabpagelocation)

-[NewTabPageSetFeedType](#newtabpagesetfeedtype)

-[SyncDisabled](#syncdisabled)

-[BrowserSignin](#browsersignin)

-[NonRemovableProfileEnabled](#nonremovableprofileenabled)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: HideFirstRunExperience
  - GP name: Hide the First-run experience and splash screen
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: HideFirstRunExperience
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: HideFirstRunExperience
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportAutofillFormData
  #### Allow importing of autofill form data
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import autofill form data from another browser into Microsoft Edge.

If you enable this policy, the option to manually import autofill data is automatically selected.

If you disable this policy, autofill form data isn't imported at first run, and users can't import it manually.

If you don't configure this policy, autofill data is imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge will import autofill data on first run, but users can select or clear **autofill data** option during manual import.

**Note**: This policy currently manages importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportAutofillFormData
  - GP name: Allow importing of autofill form data
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportAutofillFormData
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportAutofillFormData
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportBrowserSettings
  #### Allow importing of browser settings
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Allows users to import browser settings from another browser into Microsoft Edge.

If you enable this policy, the **Browser settings** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, browser settings aren't imported at first run, and users can’t import them manually.

If you don’t configure this policy, browser settings are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports the settings on first run, but users can select or clear the **browser settings** option during manual import.

**Note**: This policy currently manages importing Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportBrowserSettings
  - GP name: Allow importing of browser settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportBrowserSettings
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportBrowserSettings
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportCookies
  #### Allow importing of Cookies
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  Allows users to import Cookies from another browser into Microsoft Edge.

If you disable this policy, Cookies aren't imported on first run.

If you don’t configure this policy, Cookies are imported on first run.

You can also set this policy as a recommendation. This means that Microsoft Edge imports Cookies on first run.

**Note**: This policy currently manages importing Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportCookies
  - GP name: Allow importing of Cookies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportCookies
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportCookies
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportExtensions
  #### Allow importing of extensions
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  Allows users to import extensions from another browser into Microsoft Edge.

If you enable this policy, the **Extensions** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, extensions aren't imported at first run, and users can't import them manually.

If you don't configure this policy, extensions are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports extensions on first run, but users can select or clear the **favorites** option during manual import.

**Note**: This policy currently only supports importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportExtensions
  - GP name: Allow importing of extensions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportExtensions
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportExtensions
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportFavorites
  #### Allow importing of favorites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import favorites from another browser into Microsoft Edge.

If you enable this policy, the **Favorites** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, favorites aren't imported at first run, and users can’t import them manually.

If you don’t configure this policy, favorites are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports favorites on first run, but users can select or clear the **favorites** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (on macOS) browsers.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportFavorites
  - GP name: Allow importing of favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportFavorites
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportFavorites
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportHistory
  #### Allow importing of browsing history
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import their browsing history from another browser into Microsoft Edge.

If you enable this policy, the **Browsing history** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, browsing history data isn't imported at first run, and users can’t import this data manually.

If you don’t configure this policy, browsing history data is imported at first run, and users can choose whether to import it manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports browsing history on first run, but users can select or clear the **history** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (macOS) browsers.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportHistory
  - GP name: Allow importing of browsing history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportHistory
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportHistory
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportHomepage
  #### Allow importing of home page settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import their home page setting from another browser into Microsoft Edge.

If you enable this policy, the option to manually import the home page setting is automatically selected.

If you disable this policy, the home page setting isn’t imported at first run, and users can’t import it manually.

If you don’t configure this policy, the home page setting is imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports the home page setting on first run, but users can select or clear the **home page** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportHomepage
  - GP name: Allow importing of home page settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ImportHomepage
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportHomepage
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportOpenTabs
  #### Allow importing of open tabs
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Allows users to import open and pinned tabs from another browser into Microsoft Edge.

If you enable this policy, the **Open tabs** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, open tabs aren't imported at first run, and users can't import them manually.

If you don't configure this policy, open tabs are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports open tabs on first run, but users can select or clear the **Open tabs** option during manual import.

**Note**: This policy currently only supports importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportOpenTabs
  - GP name: Allow importing of open tabs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportOpenTabs
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportOpenTabs
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportPaymentInfo
  #### Allow importing of payment info
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import payment info from another browser into Microsoft Edge.

If you enable this policy, the **payment info** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, payment info isn’t imported at first run, and users can’t import it manually.

If you don’t configure this policy, payment info is imported at first run, and users can choose whether to import it manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports payment info on first run, but users can select or clear the **payment info** option during manual import.

**Note:** This policy currently manages importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportPaymentInfo
  - GP name: Allow importing of payment info
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportPaymentInfo
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportPaymentInfo
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportSavedPasswords
  #### Allow importing of saved passwords
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import saved passwords from another browser into Microsoft Edge.

If you enable this policy, the option to manually import saved passwords is automatically selected.

If you disable this policy, saved passwords aren't imported on first run, and users can't import them manually.

If you don't configure this policy, passwords are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports passwords on first run, but users can select or clear the **passwords** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10) and Google Chrome (on Windows 7, 8, and 10 and on macOS) browsers.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportSavedPasswords
  - GP name: Allow importing of saved passwords
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportSavedPasswords
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportSavedPasswords
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportSearchEngine
  #### Allow importing of search engine settings
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows users to import search engine settings from another browser into Microsoft Edge.

If you enable, this policy, the option to import search engine settings is automatically selected.

If you disable this policy, search engine settings aren't imported at first run, and users can’t import them manually.

If you don’t configure this policy, search engine settings are imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports search engine settings on first run, but users can select or clear the **search engine** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportSearchEngine
  - GP name: Allow importing of search engine settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportSearchEngine
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportSearchEngine
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ImportShortcuts
  #### Allow importing of shortcuts
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  Allows users to import Shortcuts from another browser into Microsoft Edge.

If you disable this policy, Shortcuts aren't imported on first run.

If you don’t configure this policy, Shortcuts are imported on first run.

You can also set this policy as a recommendation. This means that Microsoft Edge imports Shortcuts on first run.

**Note**: This policy currently manages importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ImportShortcuts
  - GP name: Allow importing of shortcuts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ImportShortcuts
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ImportShortcuts
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### InPrivateModeAvailability
  #### Configure InPrivate mode availability
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies whether the user can open pages in InPrivate mode in Microsoft Edge.

If you don't configure this policy or set it to 'Enabled' (0), users can open pages in InPrivate mode.

Set this policy to 'Disable' (1) to stop users from using InPrivate mode.

Set this policy to 'Forced' (2) to always use InPrivate mode.

* 0 = InPrivate mode available

* 1 = InPrivate mode disabled

* 2 = InPrivate mode forced

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InPrivateModeAvailability
  - GP name: Configure InPrivate mode availability
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: InPrivateModeAvailability
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: InPrivateModeAvailability
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### InternetExplorerIntegrationLevel
  #### Configure Internet Explorer integration
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  For guidance about configuring the optimal experience for Internet Explorer mode see [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

* 0 = None

* 1 = Internet Explorer mode

* 2 = Internet Explorer 11

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InternetExplorerIntegrationLevel
  - GP name: Configure Internet Explorer integration
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: InternetExplorerIntegrationLevel
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### InternetExplorerIntegrationSiteList
  #### Configure the Enterprise Mode Site List
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  For guidance about configuring the optimal experience for Internet Explorer mode see [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InternetExplorerIntegrationSiteList
  - GP name: Configure the Enterprise Mode Site List
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: InternetExplorerIntegrationSiteList
  - Value Type: REG_SZ
  ##### Example value:
```
https://internal.contoso.com/sitelist.xml
```


  

  [Back to top](#microsoft-edge---policies)

  ### InternetExplorerIntegrationSiteRedirect
  #### Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages
  
  #### Supported versions:
  - On Windows since 81 or later

  #### Description
  An "in-page" navigation is started from a link, a script, or a form on the current page. It can also be a server-side redirect of a previous "in-page" navigation attempt. Conversely, a user can start a navigation that isn't "in-page" that's independent of the current page in several ways by using the browser controls. For example, using the address bar, the back button, or a favorite link.

This setting lets you specify whether navigations from pages loaded in Internet Explorer mode to unconfigured sites (that are not configured in the Enterprise Mode Site List) switch back to Microsoft Edge or remain in Internet Explorer mode.

This setting works in conjunction with:
[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel) is set to "Internet Explorer mode" (1)
and
[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist) policy where the list has at least one entry.

If you disable or don’t configure this policy, only sites configured to open in Internet Explorer mode will open in that mode. Any site not configured to open in Internet Explorer mode will be redirected back to Microsoft Edge.

If you set this policy to Default (value 0), only sites configured to open in Internet Explorer mode will open in that mode. Any site not configured to open in Internet Explorer mode will be redirected back to Microsoft Edge.

If you set this policy to AutomaticNavigationsOnly (value 1), you get the default experience except that all automatic navigations (such as 302 redirects) to unconfigured sites will be kept in Internet Explorer mode.

If you set this policy to AllInPageNavigations (value 2), all navigations from pages loaded in IE mode to unconfigured sites are kept in Internet Explorer mode (Least Recommended).

If you enable this policy, you can choose one of the following navigation options:

* 0 = Default
															
											   

* 1 = Keep only automatic navigations in Internet Explorer mode

* 2 = Keep all in-page navigations in Internet Explorer mode

To learn more about Internet Explorer mode, see [https://go.microsoft.com/fwlink/?linkid=2105106](https://go.microsoft.com/fwlink/?linkid=2105106)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: InternetExplorerIntegrationSiteRedirect
  - GP name: Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: InternetExplorerIntegrationSiteRedirect
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### IsolateOrigins
  #### Enable site isolation for specific origins
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: IsolateOrigins
  - GP name: Enable site isolation for specific origins
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: IsolateOrigins
  - Value Type: REG_SZ
  ##### Example value:
```
https://contoso.com/,https://fabrikam.com/
```


  #### Mac information and settings
  - Preference Key Name: IsolateOrigins
  - Example value:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ManagedFavorites
  #### Configure favorites
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Configures a list of managed favorites.

The policy creates a list of favorites. Each favorite contains the keys "name" and "url," which hold the favorite's name and its target. You can configure a subfolder by defining a favorites without an "url" key but with an additional "children" key that contains a list of favorites as defined above (some of which may be folders again). Microsoft Edge amends incomplete URLs as if they were submitted via the Address Bar, for example "microsoft.com" becomes "https://microsoft.com/".

These favorites are placed in a folder that can't be modified by the user (but the user can choose to hide it from the favorites bar). By default the folder name is "Managed favorites" but you can change it by adding to the list of favorites a dictionary containing the key "toplevel_name" with the desired folder name as the value.

Managed favorites are not synced to the user account and can't be modified by extensions.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ManagedFavorites
  - GP name: Configure favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ManagedFavorites
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ManagedFavorites = [
  {
    "toplevel_name": "My managed favorites folder"
  }, 
  {
    "name": "Microsoft", 
    "url": "microsoft.com"
  }, 
  {
    "name": "Bing", 
    "url": "bing.com"
  }, 
  {
    "children": [
      {
        "name": "Microsoft Edge Insiders", 
        "url": "www.microsoftedgeinsider.com"
      }, 
      {
        "name": "Microsoft Edge", 
        "url": "www.microsoft.com/windows/microsoft-edge"
      }
    ], 
    "name": "Microsoft Edge links"
  }
]
```


  #### Mac information and settings
  - Preference Key Name: ManagedFavorites
  - Example value:
``` xml
<key>ManagedFavorites</key>
<array>
  <dict>
    <key>toplevel_name</key>
    <string>My managed favorites folder</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Microsoft</string>
    <key>url</key>
    <string>microsoft.com</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Bing</string>
    <key>url</key>
    <string>bing.com</string>
  </dict>
  <dict>
    <key>children</key>
    <array>
      <dict>
        <key>name</key>
        <string>Microsoft Edge Insiders</string>
        <key>url</key>
        <string>www.microsoftedgeinsider.com</string>
      </dict>
      <dict>
        <key>name</key>
        <string>Microsoft Edge</string>
        <key>url</key>
        <string>www.microsoft.com/windows/microsoft-edge</string>
      </dict>
    </array>
    <key>name</key>
    <string>Microsoft Edge links</string>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ManagedSearchEngines
  #### Manage Search Engines
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Lets you configure a list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding. Starting in Microsoft Edge 80, the suggest_url and image_search_url parameters are optional. The optional parameter, image_search_post_params (consists of comma-separated name/value pairs), is available starting in Microsoft Edge 80.

Starting in Microsoft Edge 82, you can enable search engine discovery with the allow_search_engine_discovery optional parameter. This parameter must be the first item in the list. If allow_search_engine_discovery is not specified, search engine discovery will be disabled by default.

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policy is set, this policy (ManagedSearchEngines) is ignored. The user must restart their browser to finish applying this policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ManagedSearchEngines
  - GP name: Manage Search Engines
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ManagedSearchEngines
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\ManagedSearchEngines = [
  {
    "allow_search_engine_discovery": true
  }, 
  {
    "is_default": true, 
    "keyword": "example1.com", 
    "name": "Example1", 
    "search_url": "https://www.example1.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example1.com/qbox?query={searchTerms}"
  }, 
  {
    "image_search_post_params": "content={imageThumbnail},url={imageURL},sbisrc={SearchSource}", 
    "image_search_url": "https://www.example2.com/images/detail/search?iss=sbiupload", 
    "keyword": "example2.com", 
    "name": "Example2", 
    "search_url": "https://www.example2.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example2.com/qbox?query={searchTerms}"
  }, 
  {
    "encoding": "UTF-8", 
    "image_search_url": "https://www.example3.com/images/detail/search?iss=sbiupload", 
    "keyword": "example3.com", 
    "name": "Example3", 
    "search_url": "https://www.example3.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example3.com/qbox?query={searchTerms}"
  }, 
  {
    "keyword": "example4.com", 
    "name": "Example4", 
    "search_url": "https://www.example4.com/search?q={searchTerms}"
  }
]
```


  #### Mac information and settings
  - Preference Key Name: ManagedSearchEngines
  - Example value:
``` xml
<key>ManagedSearchEngines</key>
<array>
  <dict>
    <key>allow_search_engine_discovery</key>
    <true/>
  </dict>
  <dict>
    <key>is_default</key>
    <true/>
    <key>keyword</key>
    <string>example1.com</string>
    <key>name</key>
    <string>Example1</string>
    <key>search_url</key>
    <string>https://www.example1.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example1.com/qbox?query={searchTerms}</string>
  </dict>
  <dict>
    <key>image_search_post_params</key>
    <string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
    <key>image_search_url</key>
    <string>https://www.example2.com/images/detail/search?iss=sbiupload</string>
    <key>keyword</key>
    <string>example2.com</string>
    <key>name</key>
    <string>Example2</string>
    <key>search_url</key>
    <string>https://www.example2.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example2.com/qbox?query={searchTerms}</string>
  </dict>
  <dict>
    <key>encoding</key>
    <string>UTF-8</string>
    <key>image_search_url</key>
    <string>https://www.example3.com/images/detail/search?iss=sbiupload</string>
    <key>keyword</key>
    <string>example3.com</string>
    <key>name</key>
    <string>Example3</string>
    <key>search_url</key>
    <string>https://www.example3.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example3.com/qbox?query={searchTerms}</string>
  </dict>
  <dict>
    <key>keyword</key>
    <string>example4.com</string>
    <key>name</key>
    <string>Example4</string>
    <key>search_url</key>
    <string>https://www.example4.com/search?q={searchTerms}</string>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### MaxConnectionsPerProxy
  #### Maximum number of concurrent connections to the proxy server
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies the maximum number of simultaneous connections to the proxy server.

Some proxy servers can't handle a high number of concurrent connections per client - you can solve this by setting this policy to a lower value.

The value of this policy should be lower than 100 and higher than 6. The default value is 32.

Some web apps are known to consume many connections with hanging GETs - lowering the maximum connections below 32 may lead to browser networking hangs if too many of these kind of web apps are open.

If you don't configure this policy, the default value (32) is used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: MaxConnectionsPerProxy
  - GP name: Maximum number of concurrent connections to the proxy server
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: MaxConnectionsPerProxy
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000020
```


  #### Mac information and settings
  - Preference Key Name: MaxConnectionsPerProxy
  - Example value:
``` xml
<integer>32</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### MediaRouterCastAllowAllIPs
  #### Allow Google Cast to connect to Cast devices on all IP addresses
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the [EnableMediaRouter](#enablemediarouter) policy is disabled, then this policy has no effect.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: MediaRouterCastAllowAllIPs
  - GP name: Allow Google Cast to connect to Cast devices on all IP addresses
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: MediaRouterCastAllowAllIPs
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: MediaRouterCastAllowAllIPs
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### MetricsReportingEnabled
  #### Enable usage and crash-related data reporting
	   

   
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  This policy enables reporting of usage and crash-related data about Microsoft Edge to Microsoft.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, Beta and Stable channels, if you don’t configure this policy, Microsoft Edge will default to the Windows diagnostic data setting. If you enable this policy, Microsoft Edge will only send usage data if the Windows Diagnostic data setting is set to Enhanced or Full. If you disable this policy, Microsoft Edge will not send usage data. Crash-related data is sent based on the Windows Diagnostic data setting. Learn more about Windows Diagnostic data settings at [https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)

 

On Windows 10, Canary and Dev channels, this policy controls sending usage data. If this policy is not configured, Microsoft Edge will default to the user's preference. Crash-related data is sent based on the Windows Diagnostic data setting. Learn more about Windows Diagnostic data settings: [https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)

On Windows 7, 8, and macOS, this policy controls sending usage and crash-related data. If you don’t configure this policy, Microsoft Edge will default to the user's preference.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: MetricsReportingEnabled
  - GP name: Enable usage and crash-related data reporting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: MetricsReportingEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: MetricsReportingEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NativeWindowOcclusionEnabled
  #### Enable Hiding of Native Windows
  
  #### Supported versions:
  - On Windows since 82 or later

  #### Description
  Enables hiding of native windows in Microsoft Edge.

If you enable this setting, to reduce CPU and power consumption Microsoft Edge will detect when a window is covered by other windows, and will suspend work painting pixels.

If you disable this setting Microsoft Edge will not detect when a window is covered by other windows.

If this policy is left not set, window hiding detection will be enabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NativeWindowOcclusionEnabled
  - GP name: Enable Hiding of Native Windows
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: NativeWindowOcclusionEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### NetworkPredictionOptions
  #### Enable network prediction
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables network prediction and prevents users from changing this setting.

This controls DNS prefetching, TCP and SSL preconnection, and prerendering of web pages.

If you don't configure this policy, network prediction is enabled but the user can change it.

* 0 = Predict network actions on any network connection

* 2 = Don't predict network actions on any network connection

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NetworkPredictionOptions
  - GP name: Enable network prediction
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: NetworkPredictionOptions
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: NetworkPredictionOptions
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### NonRemovableProfileEnabled
  #### Configure whether a user always has a default profile automatically signed in with their work or school account
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  This policy determines if a user can remove the Microsoft Edge profile automatically signed in with a user's work or school account.

If you enable this policy, a non-removable profile will be created with the user's work or school account on Windows. This profile can't be signed out or removed.

If you disable or don't configure this policy, the profile automatically signed in with a user's work or school account on Windows can be signed out or removed by the user.

If you want to configure browser sign in, use the [BrowserSignin](#browsersignin) policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: NonRemovableProfileEnabled
  - GP name: Configure whether a user always has a default profile automatically signed in with their work or school account
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: NonRemovableProfileEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

 

 
   
 

   
  

   

   

  
 
  
 

  
   

   
  
   
   
  
   
 
   
   
   
  
 
 
   
 
   


  
  
   
 
 
   
  

  [Back to top](#microsoft-edge---policies)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Control where security restrictions on insecure origins apply
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies a list of origins (URLs) or hostname patterns (like "*.contoso.com") for which security restrictions on insecure origins don't apply.

This policy lets you specify allowed origins for legacy applications that can't deploy TLS or set up a staging server for internal web development so that developers can test out features requiring secure contexts without having to deploy TLS on the staging server. This policy also prevents the origin from being labeled "Not Secure" in the omnibox.

Setting a list of URLs in this policy has the same effect as setting the command-line flag '--unsafely-treat-insecure-origin-as-secure' to a comma-separated list of the same URLs. If you enable this policy, it overrides the command-line flag.

For more information on secure contexts, see https://www.w3.org/TR/secure-contexts/.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: OverrideSecurityRestrictionsOnInsecureOrigin
  - GP name: Control where security restrictions on insecure origins apply
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = http://testserver.contoso.com/
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\2 = *.contoso.com

```


  #### Mac information and settings
  - Preference Key Name: OverrideSecurityRestrictionsOnInsecureOrigin
  - Example value:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PaymentMethodQueryEnabled
  #### Allow websites to query for available payment methods
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Allows you to set whether websites can check if the user has payment methods saved.

If you disable this policy, websites that use PaymentRequest.canMakePayment or PaymentRequest.hasEnrolledInstrument API will be informed that no payment methods are available.

If you enable this policy or don't set this policy, websites can check if the user has payment methods saved.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PaymentMethodQueryEnabled
  - GP name: Allow websites to query for available payment methods
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PaymentMethodQueryEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PaymentMethodQueryEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PersonalizationReportingEnabled
  #### Allow personalization of ads, search and news by sending browsing history to Microsoft
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  This policy prevents Microsoft from collecting a user's Microsoft Edge browsing history to be used for personalizing advertising, search, news and other Microsoft services.

This setting is only available for users with a Microsoft account. This setting is not available for child accounts or enterprise accounts.

If you disable this policy, users can't change or override the setting. If this policy is enabled or not configured, Microsoft Edge will default to the user’s preference.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PersonalizationReportingEnabled
  - GP name: Allow personalization of ads, search and news by sending browsing history to Microsoft
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PersonalizationReportingEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: PersonalizationReportingEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PinningWizardAllowed
  #### Allow Pin to taskbar wizard
  
  #### Supported versions:
  - On Windows since 80 or later

  #### Description
  Microsoft Edge uses the Pin to taskbar wizard to help users pin suggested sites to the taskbar. The Pin to taskbar wizard feature is enabled by default and accessible to the user through the Settings and more menu.

If you enable this policy or don't configure it, users can call the Pin to taskbar wizard from the Settings and More menu. The wizard can also be called via a protocol launch.

If you disable this policy, the Pin to taskbar wizard is disabled in the menu and cannot be called via a protocol launch.

User settings to enable or disable the Pin to taskbar wizard aren't available.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PinningWizardAllowed
  - GP name: Allow Pin to taskbar wizard
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PinningWizardAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### ProactiveAuthEnabled
  #### Enable Proactive Authentication
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Lets you configure whether to turn on Proactive Authentication.

If you enable this policy, Microsoft Edge tries to proactively authenticate the signed-in user with Microsoft services. At regular intervals, Microsoft Edge checks with an online service for an updated manifest that contains the configuration that governs how to do this.

If you disable this policy, Microsoft Edge doesn't try to proactively authenticate the signed-in user with Microsoft services. Microsoft Edge no longer checks with an online service for an updated manifest that contains the configuration for doing this.

If you don't configure this policy, Proactive Authentication is turned on.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ProactiveAuthEnabled
  - GP name: Enable Proactive Authentication
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ProactiveAuthEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ProactiveAuthEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PromotionalTabsEnabled
  #### Enable full-tab promotional content
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Control the presentation of full-tab promotional or educational content. This setting controls the presentation of welcome pages that help users sign into Microsoft Edge, choose their default browser, or learn about product features.

If you enable this policy (set it true) or don't configure it, Microsoft Edge can show full-tab content to users to provide product information.

If you disable (set to false) this policy, Microsoft Edge can't show full-tab content to users.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PromotionalTabsEnabled
  - GP name: Enable full-tab promotional content
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PromotionalTabsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: PromotionalTabsEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### PromptForDownloadLocation
  #### Ask where to save downloaded files
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set whether to ask where to save a file before downloading it.

If you enable this policy, the user is asked where to save each file before downloading; if you don't configure it, files are saved automatically to the default location, without asking the user.

If you don't configure this policy, the user will be able to change this setting.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: PromptForDownloadLocation
  - GP name: Ask where to save downloaded files
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: PromptForDownloadLocation
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: PromptForDownloadLocation
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### QuicAllowed
  #### Allow QUIC protocol
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows use of the QUIC protocol in Microsoft Edge.

If you enable this policy or don't configure it, the QUIC protocol is allowed.

If you disable this policy, the QUIC protocol is blocked.

QUIC is a transport layer network protocol that can improve performance of web applications that currently use TCP.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: QuicAllowed
  - GP name: Allow QUIC protocol
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: QuicAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: QuicAllowed
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RelaunchNotification
  #### Notify a user that a browser restart is recommended or required for pending updates
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the [RelaunchNotificationPeriod](#relaunchnotificationperiod) policy.

The user's session is restored when the browser restarts.

* 1 = Recommended - Show a recurring prompt to the user indicating that a restart is recommended

* 2 = Required - Show a recurring prompt to the user indicating that a restart is required

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RelaunchNotification
  - GP name: Notify a user that a browser restart is recommended or required for pending updates
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RelaunchNotification
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: RelaunchNotification
  - Example value:
``` xml
<integer>1</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RelaunchNotificationPeriod
  #### Set the time period for update notifications
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to set the time period, in milliseconds, over which users are notified that Microsoft Edge must be relaunched or that a Microsoft Edge OS device must be restarted to apply a pending update.

Over this time period, the user will be repeatedly informed of the need for an update. For Microsoft Edge OS devices, a restart notification appears in the system tray according to the RelaunchHeadsUpPeriod policy. For Microsoft Edge browsers, the app menu changes to indicate that a relaunch is needed once one third of the notification period passes. This notification changes color once two thirds of the notification period passes, and again once the full notification period has passed. The additional notifications enabled by the [RelaunchNotification](#relaunchnotification) policy follow this same schedule.

If not set, the default period of 604800000 milliseconds (one week) is used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RelaunchNotificationPeriod
  - GP name: Set the time period for update notifications
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RelaunchNotificationPeriod
  - Value Type: REG_DWORD
  ##### Example value:
```
0x240c8400
```


  #### Mac information and settings
  - Preference Key Name: RelaunchNotificationPeriod
  - Example value:
``` xml
<integer>604800000</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RendererCodeIntegrityEnabled
  #### Enable renderer code integrity
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  If this policy is enabled or left unset, then Renderer Code Integrity is enabled. This policy should only be disabled if compatibility issues are encountered with third party software that must run inside Microsoft Edge's renderer processes.

Disabling this policy has a detrimental effect on Microsoft Edge's security and stability because unknown and potentially hostile code will be allowed to load inside Microsoft Edge's renderer processes.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RendererCodeIntegrityEnabled
  - GP name: Enable renderer code integrity
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RendererCodeIntegrityEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Specify if online OCSP/CRL checks are required for local trust anchors
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  Control whether online revocation checks (OCSP/CRL checks) are required. If Microsoft Edge can't get revocation status information, these certificates are treated as revoked ("hard-fail").

If you enable this policy, Microsoft Edge always performs revocation checking for server certificates that successfully validate and are signed by locally-installed CA certificates.

If you don't configure or disable this policy, then Microsoft Edge uses the existing online revocation checking settings.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RequireOnlineRevocationChecksForLocalAnchors
  - GP name: Specify if online OCSP/CRL checks are required for local trust anchors
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RequireOnlineRevocationChecksForLocalAnchors
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  

  [Back to top](#microsoft-edge---policies)

  ### ResolveNavigationErrorsUseWebService
  #### Enable resolution of navigation errors using a web service
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ResolveNavigationErrorsUseWebService
  - GP name: Enable resolution of navigation errors using a web service
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: ResolveNavigationErrorsUseWebService
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: ResolveNavigationErrorsUseWebService
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RestrictSigninToPattern
  #### Restrict which accounts can be used as Microsoft Edge primary accounts
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Determines which accounts can be set as browser primary accounts in Microsoft Edge (the account that is chosen during the Sync opt-in flow).

One or more accounts can be configured for this policy according to the pattern/regular expression (regex) used.

If a user tries to set a browser primary account with a username that doesn't match this pattern, they are blocked and see an appropriate error message.

If you don't configure this policy or leave it blank, users can set any account as a browser primary account in Microsoft Edge.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RestrictSigninToPattern
  - GP name: Restrict which accounts can be used as Microsoft Edge primary accounts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RestrictSigninToPattern
  - Value Type: REG_SZ
  ##### Example value:
```
.*@(contoso1\.com|contoso2\.com)
```


  #### Mac information and settings
  - Preference Key Name: RestrictSigninToPattern
  - Example value:
``` xml
<string>.*@(contoso1\.com|contoso2\.com)</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### RunAllFlashInAllowMode
  #### Extend Adobe Flash content setting to all content
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls), and [PluginsBlockedForUrls](#pluginsblockedforurls) policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: RunAllFlashInAllowMode
  - GP name: Extend Adobe Flash content setting to all content
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: RunAllFlashInAllowMode
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: RunAllFlashInAllowMode
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SSLErrorOverrideAllowed
  #### Allow users to proceed from the HTTPS warning page
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Microsoft Edge shows a warning page when users visit sites that have SSL errors.

If you enable or don't configure (default) this policy, users can click through these warning pages.

If you disable this policy, users are blocked from clicking through any warning page.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SSLErrorOverrideAllowed
  - GP name: Allow users to proceed from the HTTPS warning page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SSLErrorOverrideAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SSLErrorOverrideAllowed
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SSLVersionMin
  #### Minimum TLS version enabled
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Sets the minimum supported version of SSL. If you don't configure this policy, Microsoft Edge uses a default minimum version, TLS 1.0.

If you enable this policy, you can set the minimum version to one of the following values: "tls1", "tls1.1" or "tls1.2". When set, Microsoft Edge won't use any version of SSL/TLS lower than the specified version. Any unrecognized value is ignored.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SSLVersionMin
  - GP name: Minimum TLS version enabled
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SSLVersionMin
  - Value Type: REG_SZ
  ##### Example value:
```
tls1
```


  #### Mac information and settings
  - Preference Key Name: SSLVersionMin
  - Example value:
``` xml
<string>tls1</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SavingBrowserHistoryDisabled
  #### Disable saving browser history
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables saving browser history and prevents users from changing this setting.

If you enable this policy, browsing history isn't saved. This also disables tab syncing.

If you disable this policy or don't configure it, browsing history is saved.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SavingBrowserHistoryDisabled
  - GP name: Disable saving browser history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SavingBrowserHistoryDisabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SavingBrowserHistoryDisabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ScreenCaptureAllowed
  #### Allow or deny screen capture
  
  #### Supported versions:
  - On Windows and macOS since 83 or later

  #### Description
  If you enable this policy, or don't configure this policy, a web page can use screen-share APIs (for example, getDisplayMedia() or the Desktop Capture extension API) for a screen capture.
If you disable this policy, calls to screen-share APIs will fail. For example, if you're using a web-based online meeting, video or screen sharing will not work.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ScreenCaptureAllowed
  - GP name: Allow or deny screen capture
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ScreenCaptureAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ScreenCaptureAllowed
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ScrollToTextFragmentEnabled
  #### Enable scrolling to text specified in URL fragments
  
  #### Supported versions:
  - On Windows and macOS since 82 or later

  #### Description
  This feature lets hyperlink and address bar URL navigations target specific text on a web page, which will be scrolled to after the web page finishes loading.
​
If you enable or don't configure this policy, web page scrolling to specific text fragments via a URL will be enabled.​

If you disable this policy, web page scrolling to specific text fragments via a URL will be disabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ScrollToTextFragmentEnabled
  - GP name: Enable scrolling to text specified in URL fragments
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ScrollToTextFragmentEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ScrollToTextFragmentEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SearchSuggestEnabled
  #### Enable search suggestions
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables web search suggestions in Microsoft Edge's Address Bar and Auto-Suggest List and prevents users from changing this policy.

If you enable this policy, web search suggestions are used.

If you disable this policy, web search suggestions are never used, however local history and local favorites suggestions still appear. If you disable this policy, neither the typed characters, nor the URLs visited will be included in telemetry to Microsoft.

If this policy is left not set, search suggestions are enabled but the user can change that.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SearchSuggestEnabled
  - GP name: Enable search suggestions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: SearchSuggestEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SearchSuggestEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SecurityKeyPermitAttestation
  #### Websites or domains that don't need permission to use direct Security Key attestation
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies websites and domains that don't need explicit user permission when attestation certificates from security keys are requested. Additionally, a signal is sent to the security key indicating that it can use individual attestation. Without this, users are prompted each time a site requests attestation of security keys.

Sites (like https://contoso.com/some/path) only match as U2F appIDs. Domains (like contoso.com) only match as webauthn RP IDs. To cover both U2F and webauthn APIs for a given site, you need to list both the appID URL and domain.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SecurityKeyPermitAttestation
  - GP name: Websites or domains that don't need permission to use direct Security Key attestation
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\1 = https://contoso.com

```


  #### Mac information and settings
  - Preference Key Name: SecurityKeyPermitAttestation
  - Example value:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SendIntranetToInternetExplorer
  #### Send all intranet sites to Internet Explorer
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  For guidance about configuring the optimal experience for Internet Explorer mode see [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SendIntranetToInternetExplorer
  - GP name: Send all intranet sites to Internet Explorer
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SendIntranetToInternetExplorer
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  

  [Back to top](#microsoft-edge---policies)

  ### SendSiteInfoToImproveServices
  #### Send site information to improve Microsoft services
	   

   
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  This policy enables sending info about websites visited in Microsoft Edge to Microsoft to improve services like search.

 

Enable this policy to send info about websites visited in Microsoft Edge to Microsoft. Disable this policy to not send info about websites visited in Microsoft Edge to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, Beta and Stable if this policy is not configured, Microsoft Edge will default to the Windows diagnostic data setting. If this policy is enabled Microsoft Edge will only send info about websites visited in Microsoft Edge if the Windows Diagnostic data setting is set to Full. If this policy is disabled Microsoft Edge will not send info about websites visited. Learn more about Windows Diagnostic data settings: [https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)

On Windows 10, Canary and Dev channels, this policy controls sending info about websites visited. If this policy is not configured, Microsoft Edge will default to the user’s preference.

On Windows 7, 8, and Mac this policy controls sending info about websites visited. If this policy is not configured, Microsoft Edge will default to the user’s preference.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SendSiteInfoToImproveServices
  - GP name: Send site information to improve Microsoft services
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SendSiteInfoToImproveServices
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: SendSiteInfoToImproveServices
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### ShowOfficeShortcutInFavoritesBar
  #### Show Microsoft Office shortcut in favorites bar
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specifies whether to include a shortcut to Office.com in the favorites bar. For users signed into Microsoft Edge the shortcut takes users to their Microsoft Office apps and docs.

If this policy is enabled or not configure, users can choose whether to see the shortcut by changing the toggle in the favorites bar context menu.

If the policy is disabled, the shortcut won't be shown.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: ShowOfficeShortcutInFavoritesBar
  - GP name: Show Microsoft Office shortcut in favorites bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: ShowOfficeShortcutInFavoritesBar
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: ShowOfficeShortcutInFavoritesBar
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SignedHTTPExchangeEnabled
  #### Enable Signed HTTP Exchange (SXG) support
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Enable support for Signed HTTP Exchange (SXG).

If this policy isn't set or enabled, Microsoft Edge will accept web contents served as Signed HTTP Exchanges.

If this policy is set to disabled, Signed HTTP Exchanges can't be loaded.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SignedHTTPExchangeEnabled
  - GP name: Enable Signed HTTP Exchange (SXG) support
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SignedHTTPExchangeEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SignedHTTPExchangeEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SitePerProcess
  #### Enable site isolation for every site
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  
The 'SitePerProcess' policy can be used to prevent users from opting out of the default behavior of isolating all sites. Note that you can also use the [IsolateOrigins](#isolateorigins) policy to isolate additional, finer-grained origins.
If you enable this policy, users can't opt out of the default behavior where each site runs in its own process.
If you disable or don’t configure this policy, a user can opt out of site isolation.  (For example, by using "Disable site isolation" entry in edge://flags.)  Disabling the policy or not configuring the policy doesn't turn off Site Isolation.


  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SitePerProcess
  - GP name: Enable site isolation for every site
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SitePerProcess
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SitePerProcess
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SpellcheckEnabled
  #### Enable spellcheck
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](#spellchecklanguage) and [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policies are also disabled.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SpellcheckEnabled
  - GP name: Enable spellcheck
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SpellcheckEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: SpellcheckEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SpellcheckLanguage
  #### Enable specific spellcheck languages
  
  #### Supported versions:
  - On Windows since 77 or later

  #### Description
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policy, the spellcheck language is enabled.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SpellcheckLanguage
  - GP name: Enable specific spellcheck languages
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = fr
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\2 = es

```


  

  [Back to top](#microsoft-edge---policies)

  ### SpellcheckLanguageBlocklist
  #### Force disable spellcheck languages
  
  #### Supported versions:
  - On Windows since 78 or later

  #### Description
  Force-disables spellcheck languages. Unrecognized languages in that list will be ignored.

If you enable this policy, spellcheck will be disabled for the languages specified. The user can still enable or disable spellcheck for languages not in the list.

If you do not set this policy, or disable it, there will be no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is set to disabled, this policy will have no effect.

If a language is included in both the [SpellcheckLanguage](#spellchecklanguage) and the 'SpellcheckLanguageBlocklist' policy, the spellcheck language is enabled.

The currently supported languages are: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SpellcheckLanguageBlocklist
  - GP name: Force disable spellcheck languages
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = fr
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\2 = es

```


  

  [Back to top](#microsoft-edge---policies)

  ### StricterMixedContentTreatmentEnabled
  #### Enable stricter treatment for mixed content
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  This policy controls the treatment for mixed content (HTTP content in HTTPS sites) in the browser.

If you set this policy to true or not set, audio and video mixed content will be automatically upgraded to HTTPS (that is, the URL will be rewritten as HTTPS, without a fallback if the resource isn’t available over HTTPS) and a 'Not Secure' warning will be shown in the URL bar for image mixed content.

If you set the policy to false, auto upgrades will be disabled for audio and video, and no warning will be shown for images.

This policy does not affect other types of mixed content other than audio, video, and images.

This policy will no longer take effect starting in Microsoft Edge 84.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: StricterMixedContentTreatmentEnabled
  - GP name: Enable stricter treatment for mixed content
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: StricterMixedContentTreatmentEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: StricterMixedContentTreatmentEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SuppressUnsupportedOSWarning
  #### Suppress the unsupported OS warning
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Suppresses the warning that appears when Microsoft Edge is running on a computer or operating system that is no longer supported.

If this policy is false or unset, the warnings will appear on such unsupported computers or operating systems.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SuppressUnsupportedOSWarning
  - GP name: Suppress the unsupported OS warning
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: SuppressUnsupportedOSWarning
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SuppressUnsupportedOSWarning
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### SyncDisabled
  #### Disable synchronization of data using Microsoft sync services
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Disables data synchronization in Microsoft Edge. This policy also prevents the sync consent prompt from appearing.

   

If you don't set this policy or apply it as recommended, users will be able to turn sync on or off. If you apply this policy as mandatory, users will not be able to turn sync on.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: SyncDisabled
  - GP name: Disable synchronization of data using Microsoft sync services
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: SyncDisabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: SyncDisabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TLS13HardeningForLocalAnchorsEnabled
  #### Enable a TLS 1.3 security feature for local trust anchors.
  
  #### Supported versions:
  - On Windows and macOS since 81 or later

  #### Description
  This policy controls a security feature in TLS 1.3 that protects connections against downgrade attacks. It is backwards-compatible and will not affect connections to compliant TLS 1.2 servers or proxies. However, older versions of some TLS-intercepting proxies have an implementation flaw which causes them to be incompatible.

If you set this policy to True, Microsoft Edge will enable these security protections for all connections.

If you set this policy to False or don’t set it, Microsoft Edge will disable these security protections for connections authenticated with locally-installed CA certificates. These protections are always enabled for connections authenticated with publicly-trusted CA certificates.

This policy may be used to test for any affected proxies and upgrade them. Affected proxies are expected to fail connections with an error code of ERR_TLS13_DOWNGRADE_DETECTED. A later version of Microsoft Edge will enable this option by default.

After it is enabled by default, administrators who need more time to upgrade affected proxies may use this policy to temporarily disable this security feature. This policy will be removed after version 85.


  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TLS13HardeningForLocalAnchorsEnabled
  - GP name: Enable a TLS 1.3 security feature for local trust anchors.
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: TLS13HardeningForLocalAnchorsEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: TLS13HardeningForLocalAnchorsEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TabFreezingEnabled
  #### Allow freezing of background tabs
  
  #### Supported versions:
  - On Windows and macOS since 79 or later

  #### Description
  Controls whether Microsoft Edge can freeze tabs that are in the background for at least 5 minutes.

Tab freezing reduces CPU, battery, and memory usage. Microsoft Edge uses heuristics to avoid freezing tabs that do useful work in the background, such as display notifications, play sound, and stream video.

If you enable or don't configure this policy, tabs that have been in the background for at least 5 minutes might be frozen.

If you disable this policy, no tabs will be frozen.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TabFreezingEnabled
  - GP name: Allow freezing of background tabs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: TabFreezingEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: TabFreezingEnabled
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TaskManagerEndProcessEnabled
  #### Enable ending processes in the Browser task manager
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  If you enable or don't configure this policy, users can end processes in the Browser task manager. If you disable it, users can't end processes, and the End process button is disabled in the Browser task manager.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TaskManagerEndProcessEnabled
  - GP name: Enable ending processes in the Browser task manager
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: TaskManagerEndProcessEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: TaskManagerEndProcessEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TotalMemoryLimitMb
  #### Set limit on megabytes of memory a single Microsoft Edge instance can use.
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Configures the amount of memory that a single Microsoft Edge instance can use before tabs start getting discarded to save memory. The memory used by the tab will be freed and the tab will have to be reloaded when switched to.

If you enable this policy, the browser will start to discard tabs to save memory once the limitation is exceeded. However, there is no guarantee that the browser is always running under the limit. Any value under 1024 will be rounded up to 1024.

If you don't set this policy, the browser will only attempt to save memory when it has detected that the amount of physical memory on its machine is low.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TotalMemoryLimitMb
  - GP name: Set limit on megabytes of memory a single Microsoft Edge instance can use.
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: TotalMemoryLimitMb
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000800
```


  #### Mac information and settings
  - Preference Key Name: TotalMemoryLimitMb
  - Example value:
``` xml
<integer>2048</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TrackingPrevention
  #### Block tracking of users' web-browsing activity
  
  #### Supported versions:
  - On Windows and macOS since 78 or later

  #### Description
  Lets you decide whether to block websites from tracking users' web-browsing activity.

If you enable this policy, you have the following options for setting the level of tracking prevention:

* 0 = Off (no tracking prevention)
				   
								 
										   

* 1 = Basic (blocks harmful trackers, content and ads will be personalized)

* 2 = Balanced (blocks harmful trackers and trackers from sites user has not visited; content and ads will be less personalized)

* 3 = Strict (blocks harmful trackers and majority of trackers from all sites; content and ads will have minimal personalization. Some parts of sites might not work)

If you disable this policy or don't configure it, users can set their own level of tracking prevention.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Integer

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TrackingPrevention
  - GP name: Block tracking of users' web-browsing activity
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: TrackingPrevention
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000002
```


  #### Mac information and settings
  - Preference Key Name: TrackingPrevention
  - Example value:
``` xml
<integer>2</integer>
```
  

  [Back to top](#microsoft-edge---policies)

  ### TranslateEnabled
  #### Enable Translate
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Enables the integrated Microsoft translation service on Microsoft Edge.

If you enable this policy, Microsoft Edge offers translation functionality to the user by showing an integrated translate flyout when appropriate, and a translate option on the right-click context menu.

Disable this policy to disable all built-in translate features.

If you don't configure the policy, users can choose whether to use the translation functionality or not.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: TranslateEnabled
  - GP name: Enable Translate
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name: TranslateEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: TranslateEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### URLAllowlist
  #### Define a list of allowed URLs
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the [URLBlocklist](#urlblocklist) policy.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: URLAllowlist
  - GP name: Define a list of allowed URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = contoso.com
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = https://ssl.server.com
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = hosting.com/good_path
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = https://server:8080/path
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\5 = .exact.hostname.com

```


  #### Mac information and settings
  - Preference Key Name: URLAllowlist
  - Example value:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### URLBlocklist
  #### Block access to a list of URLs
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can define exceptions in the [URLAllowlist](#urlallowlist) policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: URLBlocklist
  - GP name: Block access to a list of URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\1 = contoso.com
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\2 = https://ssl.server.com
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\3 = hosting.com/bad_path
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\4 = https://server:8080/path
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\5 = .exact.hostname.com
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\6 = file://*
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\7 = custom_scheme:*
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\8 = *

```


  #### Mac information and settings
  - Preference Key Name: URLBlocklist
  - Example value:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/bad_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
  <string>file://*</string>
  <string>custom_scheme:*</string>
  <string>*</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### UserDataDir
  #### Set the user data directory
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Set the directory to use for storing user data.

If you enable this policy, Microsoft Edge uses the specified directory regardless of whether the user has set the '--user-data-dir' command-line flag.

If you don't enable this policy, the default profile path is used, but the user can override it by using the '--user-data-dir' flag. Users can find the directory for the profile at edge://version/ under profile path.

To avoid data loss or other errors, don't configure this policy to a volume's root directory or to a directory that's used for other purposes, because Microsoft Edge manages its contents.

See [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) for a list of variables that can be used.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: UserDataDir
  - GP name: Set the user data directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: UserDataDir
  - Value Type: REG_SZ
  ##### Example value:
```
${users}/${user_name}/Edge
```


  #### Mac information and settings
  - Preference Key Name: UserDataDir
  - Example value:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### UserFeedbackAllowed
  #### Allow user feedback
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Microsoft Edge uses the Edge Feedback feature (enabled by default) to allow users to send feedback, suggestions or customer surveys and to report any issues with the browser. Also, by default, users can't disable (turn off) the Edge Feedback feature.

If you enable this policy or don't configure it, users can invoke Edge Feedback.

If you disable this policy, users can't invoke Edge Feedback.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: UserFeedbackAllowed
  - GP name: Allow user feedback
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: UserFeedbackAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: UserFeedbackAllowed
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### VideoCaptureAllowed
  #### Allow or block video capture
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy.

This policy affects all types of video inputs, not only the built-in camera.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: VideoCaptureAllowed
  - GP name: Allow or block video capture
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: VideoCaptureAllowed
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000000
```


  #### Mac information and settings
  - Preference Key Name: VideoCaptureAllowed
  - Example value:
``` xml
<false/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### VideoCaptureAllowedUrls
  #### Sites that can access video capture devices without requesting permission
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Specify websites, based on URL patterns, that can use video capture devices without asking the user for permission. Patterns in this list are matched against the security origin of the requesting URL. If they match, the site is automatically granted access to video capture devices.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: VideoCaptureAllowedUrls
  - GP name: Sites that can access video capture devices without requesting permission
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = https://www.contoso.com/
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\2 = https://[*.]contoso.edu/

```


  #### Mac information and settings
  - Preference Key Name: VideoCaptureAllowedUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WPADQuickCheckEnabled
  #### Set WPAD optimization
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to turn off WPAD (Web Proxy Auto-Discovery) optimization in Microsoft Edge.

If you disable this policy, WPAD optimization is disabled, which makes the browser wait longer for DNS-based WPAD servers.

If you enable or don't configure the policy, WPAD optimization is enabled.

Independent of whether or how this policy is enabled, the WPAD optimization setting cannot be changed by users.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WPADQuickCheckEnabled
  - GP name: Set WPAD optimization
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WPADQuickCheckEnabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: WPADQuickCheckEnabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebAppInstallForceList
  #### Configure list of force-installed Web Apps
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Specifies a list of websites that are installed silently, without user interaction, and which can't be uninstalled or disabled by the user.

Each list item of the policy is an object with the following members:
  - "url", which is mandatory. "url" should be the URL of the web app to install.

Values for the optional members are:
  - "launch_container" should be either "window" or "tab" to indicate how the Web App will be opened after it's installed.
  - "create_desktop_shortcut" should be true if a desktop shortcut should be created on Windows.

If "default_launch_container" is omitted, the app will open in a tab by default. Regardless of the value of "default_launch_container", users can change which container the app will open in. If "create_desktop_shortcuts" is omitted, no desktop shortcuts will be created.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  #### Data Type:
  - Dictionary

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebAppInstallForceList
  - GP name: Configure list of force-installed Web Apps
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebAppInstallForceList
  - Value Type: REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\WebAppInstallForceList = [
  {
    "create_desktop_shortcut": true, 
    "default_launch_container": "window", 
    "url": "https://www.contoso.com/maps"
  }, 
  {
    "default_launch_container": "tab", 
    "url": "https://app.contoso.edu"
  }
]
```


  #### Mac information and settings
  - Preference Key Name: WebAppInstallForceList
  - Example value:
``` xml
<key>WebAppInstallForceList</key>
<array>
  <dict>
    <key>create_desktop_shortcut</key>
    <true/>
    <key>default_launch_container</key>
    <string>window</string>
    <key>url</key>
    <string>https://www.contoso.com/maps</string>
  </dict>
  <dict>
    <key>default_launch_container</key>
    <string>tab</string>
    <key>url</key>
    <string>https://app.contoso.edu</string>
  </dict>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebComponentsV0Enabled
  #### Re-enable Web Components v0 API until M84.
  >DEPRECATED: This policy is deprecated. It is currently supported but will become obsolete in a future release.
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  The Web Components v0 APIs (Shadow DOM v0, Custom Elements v0, and HTML Imports) were deprecated in 2018, and have been disabled by default starting in M80. This policy allows these features to be selectively re-enabled until M84.

     If you set this policy is set to True, the Web Components v0 features will be enabled for all sites.

     If you set this policy to False or don't set this policy, the Web Components v0 features will be disabled by default, starting in M80.

     This policy will be removed after Microsoft Edge 84.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebComponentsV0Enabled
  - GP name: Re-enable Web Components v0 API until M84. %s(deprecated)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebComponentsV0Enabled
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: WebComponentsV0Enabled
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebDriverOverridesIncompatiblePolicies
  #### Allow WebDriver to Override Incompatible Policies
  >DEPRECATED: This policy is deprecated. It is currently supported but will become obsolete in a future release.
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  
This policy was removed in M83, because it is not necessary anymore as
WebDriver is now compatible with all existing policies.

This policy allows users of the WebDriver feature to override
policies which can interfere with its operation.

Currently this policy disables [SitePerProcess](#siteperprocess) and [IsolateOrigins](#isolateorigins) policies.

If the policy is enabled, WebDriver will be able to override incomaptible
policies.
If the policy is disabled or not configured, WebDriver will not be allowed
to override incompatible policies.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - Boolean

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebDriverOverridesIncompatiblePolicies
  - GP name: Allow WebDriver to Override Incompatible Policies %s(deprecated)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebDriverOverridesIncompatiblePolicies
  - Value Type: REG_DWORD
  ##### Example value:
```
0x00000001
```


  #### Mac information and settings
  - Preference Key Name: WebDriverOverridesIncompatiblePolicies
  - Example value:
``` xml
<true/>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebRtcLocalIpsAllowedUrls
  #### Manage exposure of local IP addressess by WebRTC
  
  #### Supported versions:
  - On Windows and macOS since 80 or later

  #### Description
  Specifies a list of origins (URLs) or hostname patterns (like "*contoso.com*") for which local IP address should be exposed by WebRTC.

If you enable this policy and set a list of origins (URLs) or hostname patterns, when edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will expose the local IP address for cases that match patterns in the list.

If you disable or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will not expose local IP addresses. The local IP address is concealed with an mDNS hostname.

If you enable, disable, or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Disabled, WebRTC will expose local IP addresses.

Please note that this policy weakens the protection of local IP addresses that might be needed by administrators.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - List of strings

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebRtcLocalIpsAllowedUrls
  - GP name: Manage exposure of local IP addressess by WebRTC
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls
  - Path (Recommended): N/A
  - Value Name: 1, 2, 3, ...
  - Value Type: list of REG_SZ
  ##### Example value:
```
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\1 = https://www.contoso.com
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\2 = *contoso.com*

```


  #### Mac information and settings
  - Preference Key Name: WebRtcLocalIpsAllowedUrls
  - Example value:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>*contoso.com*</string>
</array>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebRtcLocalhostIpHandling
  #### Restrict exposure of local IP address by WebRTC
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Allows you to set whether or not WebRTC exposes the user's local IP address.

If you set this policy to "AllowAllInterfaces" ('default') or "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), WebRTC exposes the local IP address.

If you set this policy to "AllowPublicInterfaceOnly" ('default_public_interface_only') or "DisableNonProxiedUdp" ('disable_non_proxied_udp'), WebRTC doesn't expose the local IP address.

If you don't set this policy, or if you disable it, WebRTC exposes the local IP address.

  * 'default' = Allow all interfaces. This exposes the local IP address.
  * 'default_public_and_private_interfaces' = Allow public and private interfaces over http default route. This exposes the local IP address.
  * 'default_public_interface_only' = Allow public interface over http default route. This doesn't expose the local IP address.
  * 'disable_non_proxied_udp' = Use TCP unless proxy server supports UDP. This doesn't expose the local IP address.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebRtcLocalhostIpHandling
  - GP name: Restrict exposure of local IP address by WebRTC
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebRtcLocalhostIpHandling
  - Value Type: REG_SZ
  ##### Example value:
```
default
```


  #### Mac information and settings
  - Preference Key Name: WebRtcLocalhostIpHandling
  - Example value:
``` xml
<string>default</string>
```
  

  [Back to top](#microsoft-edge---policies)

  ### WebRtcUdpPortRange
  #### Restrict the range of local UDP ports used by WebRTC
  
  #### Supported versions:
  - On Windows and macOS since 77 or later

  #### Description
  Restricts the UDP port range used by WebRTC to a specified port interval (endpoints included).

By configuring this policy, you specify the range of local UDP ports that WebRTC can use.

If you don't configure this policy, or if you set it to an empty string or invalid port range, WebRTC can use any available local UDP port.

  #### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  #### Data Type:
  - String

  #### Windows information and settings
  ##### Group Policy (ADMX) info
  - GP unique name: WebRtcUdpPortRange
  - GP name: Restrict the range of local UDP ports used by WebRTC
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): N/A
  - GP ADMX file name: MSEdge.admx
  ##### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): N/A
  - Value Name: WebRtcUdpPortRange
  - Value Type: REG_SZ
  ##### Example value:
```
10000-11999
```


  #### Mac information and settings
  - Preference Key Name: WebRtcUdpPortRange
  - Example value:
``` xml
<string>10000-11999</string>
```
  

  [Back to top](#microsoft-edge---policies)


## See also
- [Configuring Microsoft Edge](configure-microsoft-edge.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Security Baselines Blog](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/bg-p/Microsoft-Security-Baselines)
