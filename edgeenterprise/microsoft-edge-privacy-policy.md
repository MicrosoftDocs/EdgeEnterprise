---
title: "Microsoft Edge privacy policy"
ms.author: likravit
author: dan-wesley
manager: srugh
ms.date: 4/29/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Using Microsoft Edge privacy policy settings"
---

# Microsoft Edge privacy policy

Microsoft is committed to providing enterprises with the information and controls needed to make choices about data collection in Microsoft Edge.

By default, Microsoft Edge deployed on non-Windows platforms doesn't send diagnostic data or site information to Microsoft.

By default, when Microsoft Edge is deployed on Windows 10, diagnostic data is sent based on the users' [Windows Diagnostic data setting](https://go.microsoft.com/fwlink/?linkid=2099569).

You can configure how Microsoft Edge handles data collection for your organization with the following group policies:

- Enable usage and crash-related data reporting.
- Send site information to improve Microsoft services.

## Policy settings

Download and use the latest Microsoft Edge Policy Template (For more information, see [Configure Microsoft Edge](configure-microsoft-edge.md).)

### Enable usage and crash-related data reporting

This policy enables reporting of usage and crash-related data about Microsoft Edge to Microsoft.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

On Windows 10 channels:

- If this policy isn't configured, Microsoft Edge will default to the Windows diagnostic data setting. 
- If this policy is enabled, Microsoft Edge will only send usage data if the Windows Diagnostic data setting is set to **Full**.
- If this policy is disabled, Microsoft Edge will not send usage data. Crash-related data is sent based on the Windows Diagnostic data setting. To [learn more about Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2099569).

On Windows 7, 8, and macOS this policy controls sending usage and crash-related data. If this policy isn't configured, Microsoft Edge will default to the user's preference.

Microsoft Edge collects a set of required data that's necessary to keep the product up to date, secure, and performing properly. This includes basic device connectivity and configuration information from Microsoft Edge about the current data collection consent, app version, and installation state about your installation of Microsoft Edge. This can be turned off by disabling the policy.

### Send site information to improve Microsoft services

This policy enables sending information about websites visited in Microsoft Edge to Microsoft to improve Microsoft products and services such as search.

Enable this policy to send information about websites visited in Microsoft Edge to Microsoft. Disable this policy to not send information about the websites that are visited in Microsoft Edge to Microsoft. In both cases, users can't change or override the setting.

On Windows 10 channels:

- If this policy isn't configured, Microsoft Edge will default to the Windows diagnostic data setting.
- If this policy is enabled, Microsoft Edge will only send information about the websites that are visited if the Windows Diagnostic data setting is set to **Full**.
- If this policy is disabled, Microsoft Edge will not send info about websites visited. To [learn more about Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2099569).

On Windows 7, 8, and macOS this policy controls sending information about the websites that are visited. If this policy isn't configured, Microsoft Edge will default to the user's preference.

## Implementation details

For Windows 10 channels to understand our implementation with the dependency on the Windows Diagnostic data setting, the following table describes our configuration if **Enable usage and crash-related data reporting** and **Send site information to improve Microsoft services** were not configured.

| Windows Diagnostic data setting | Enable usage and crash-related data reporting | Send site information to improve Microsoft services |
|---------------------------------|-----------------------------------------------|-----------------------------------------------------|
| Security                        | Not sent                                      | Not sent                                            |
| Basic                           | Not sent                                      | Not sent                                            |
| Enhanced                        | Not sent                                          | Not sent                                            |
| Full                            | Sent                                          | Sent                                                |

If your configurations for Windows 10 channels are misconfigured in accordance with this table, we will fall back to the lesser data collection setting. For example, if you set the **Enable usage and crash-related data reporting** policy to **Enabled** but the Windows Diagnostic data setting is set to **Basic**, we will not send usage and crash-related data. The correct implementation would be to set the **Enable usage and crash-related data reporting** policy to **Enabled** with the Windows Diagnostic data setting set to **Full**. Or, if you set the **Send site information to improve Microsoft services** to **Disabled** but Windows Diagnostic data setting is set to **Full**, we will not send information about the sites that are visited.  

## Additional privacy policy options

You may want to consider the following group policies related to data privacy:

- Block cookies on specific sites
- Block third-party cookies
- Configure Do Not Track
- Disable InPrivate mode

## Frequently Asked Questions

### How do I resolve Error Code -2147024540?

This error code corresponds to the following Windows Information Protection error:
*ERROR_EDP_POLICY_DENIES_OPERATION: The requested operation was blocked by Windows Information Protection policy. For more information, contact your system administrator*.

Microsoft Edge shows this error when the organization has enabled Windows Information Protection (WIP) to only allow users with approved applications to access corporate resources. In this case because Microsoft Edge isn't on the approved applications list, the admin will have to update the WIP policies to grant access to Microsoft Edge. Download and apply the policy update in the [WIP Enterprise AppLocker Policy](https://download.microsoft.com/download/8/9/9/8995d820-065c-4ab1-aa2a-9d6dc0cd7ffa/MsEdge%20-%20WIP%20Enterprise%20AppLocker%20Policy%20Files.zip) file.

> [!NOTE]
> If WIP is turned on for your version of Microsoft Edge, the browser collects event logs and sends them to your organization. To Learn more about the event logs captured by WIP, see [Windows Information Protection](https://docs.microsoft.com/microsoft-edge/privacy-whitepaper#windows-information-protection) in the Microsoft Edge Privacy Whitepaper.


## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Edge policies](microsoft-edge-policies.md)
- [Microsoft Edge Privacy Whitepaper](https://docs.microsoft.com/microsoft-edge/privacy-whitepaper)
