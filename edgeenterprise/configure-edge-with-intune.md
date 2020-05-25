---
title: "Configure Microsoft Edge policy settings for Windows using Microsoft Intune"
ms.author: kvice
author: kelleyvice-msft
manager: laurawi
ms.date: 12/13/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure Microsoft Edge policy settings for Windows using Microsoft Intune."
---

# Configure Microsoft Edge policy settings with Microsoft Intune

This article explains how to configure Microsoft Edge policy settings for Windows 10 using Microsoft Intune.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

You can configure Microsoft Edge policies and settings by adding a device configuration profile to Microsoft Intune. Using Intune to manage and enforce policies is essentially equivalent to using Active Directory Group Policy or configuring local Group Policy Object (GPO) settings on user devices.

For more information about managing Microsoft Edge policies with Microsoft Intune, you can read [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/intune/manage-microsoft-edge), but keep in mind that the linked article is specific to Microsoft Edge version 45 and earlier and therefore may contain information and references that don't apply to Microsoft Edge Enterprise version 77 and later.

> [!TIP]
> For information on how to configure Microsoft Edge on macOS using Microsoft Intune, see [Configure for macOS](configure-microsoft-edge-on-mac.md).

## Create a profile to manage settings in Microsoft Edge for Windows 10

Using Administrative Templates in Microsoft Intune, you can manage Microsoft Edge group policies on your Windows 10 devices using the cloud. This section will help you create a template to configure Microsoft Edge-specific application settings. When you create the template, it creates a device configuration profile. You can then assign or deploy this profile to Windows 10 devices in your organization.

### Prerequisites

- Windows 10 with the following minimum system requirements:
  - Windows 10, version 1903 with [KB4512941](https://support.microsoft.com/kb/4512941) installed
  - Windows 10, version 1809 with [KB4512534](https://support.microsoft.com/kb/4512534) installed
  - Windows 10, version 1803 with [KB4512509](https://support.microsoft.com/kb/4512509) installed
  - Windows 10, version 1709 with [KB4516071](https://support.microsoft.com/kb/4516071) installed

### Create an Administrative Templates profile

This procedure creates an Administrative Templates profile using Microsoft Edge policy settings built into Microsoft Intune.

1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
2. Select **Intune** from _All Services_, or search for Intune in the portal search box.
3. From the _Microsoft Intune - Overview_ blade, select **Device configuration** | **Profiles**.
4. On the top command bar, select **Create profile**.
5. Enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Microsoft Edge Policies_         |
    |Description     |Optionally enter a description         |
    |Platform     |Windows 10 and later         |
    |Profile type     |Administrative Templates         |

    ![Create profile](./media/edge-ent-intune/edge-intune-profile-create.ng)

6. Click **Settings** to show all the available settings.

    ![Create profile](./media/edge-ent-intune/edge-intune-policy-settings.png)

7. On the right upper corner of the window, select the **All products** drop-down and then select **Edge version 77 or later** to filter the list to show only Microsoft Edge settings.

    ![Create profile](./media/edge-ent-intune/edge-intune-allproducts.png)

8. To configure a setting, select it from the list and use the settings window on the right to enable and configure the setting.

    ![Create profile](./media/edge-ent-intune/edge-intune-settings-config.png)

9. Click **Create** to create the profile.

When you're finished, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/intune/device-profile-assign) for information about how to assign the profile to your Azure Active Directory (Azure AD) user or device groups.

For more information about Windows 10 profiles, see [Use Windows 10 templates to configure group policy settings in Microsoft Intune](https://docs.microsoft.com/intune/administrative-templates-windows).

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/intune/manage-microsoft-edge)
- [Use Windows 10 templates to configure group policy settings in Microsoft Intune](https://docs.microsoft.com/intune/administrative-templates-windows)
- [Deploy Microsoft Edge using Microsoft Intune](https://docs.microsoft.com/intune/apps/apps-windows-edge/?toc=https://docs.microsoft.com/DeployEdge/toc.json&bc=https://docs.microsoft.com/DeployEdge/breadcrumb/toc.json)
