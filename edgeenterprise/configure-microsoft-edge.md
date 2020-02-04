---
title: "Configure Microsoft Edge for Windows"
ms.author: brianalt
author: kelleyvice-msft
manager: laurawi
ms.date: 10/09/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure Microsoft Edge policy settings on Windows devices"
---

# Configure Microsoft Edge policy settings on Windows

Use the following information to configure Microsoft Edge policy settings on your Windows devices.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Configure policy settings on Windows

You can use _group policy objects (GPO)_ to configure policy settings for Microsoft Edge and managed Microsoft Edge updates on all versions of Windows. You can also provision policy through the registry for Windows devices that are joined to a Microsoft Active Directory domain, or Windows 10 Pro or Enterprise instances enrolled for device management in Microsoft Intune. To configure Microsoft Edge with group policy objects, you install _administrative templates_ that add rules and settings for Microsoft Edge to the group policy Central Store in your Active Directory domain or to the Policy Definition template folder on individual computers and then configure the specific policies you want to set.

You can use Active Directory group policy to configure Microsoft Edge policy settings if you prefer to manage policy at the domain level. This enables you to manage policy settings globally, targeting different policy settings to specific OUs, or using WMI filters to apply settings only to users or computers returned by a particular query. If you want to configure policy on individual computers, you can apply policy settings that only affect the local device using the Local Group Policy Editor on the target computer.

Microsoft Edge supports both _mandatory_ and _recommended_ policies. Mandatory policies override user preferences and prevents the user from changing it, while recommended policy provide a default setting that may be overridden by the user. Most policies are mandatory only; a subset are mandatory and recommended. If both versions of a policy are set, the mandatory setting takes precedence.

>[!TIP]
> You can use Microsoft Intune to configure Microsoft Edge policy settings. For more information, see [Configure Microsoft Edge using Microsoft Intune](configure-edge-with-intune.md).

There are two administrative templates for Microsoft Edge, both of which can be applied either at the computer or Active Directory domain level:

- *msedge.admx* to [configure Microsoft Edge settings](microsoft-edge-policies.md)
- *msedgeupdate.admx* to [manage Microsoft Edge updates](microsoft-edge-update-policies.md).

To get started, download and install the Microsoft Edge administrative template.

### 1. Download and install the Microsoft Edge administrative template

If you want to configure Microsoft Edge policy settings in Active Directory, download the files to a network location you can access from a domain controller or a workstation with the Remote Server Administration Tools (RSAT) installed. To configure on an individual computer, simply download the files to that computer.

When you add the administrative template files to the appropriate location, Microsoft Edge policy settings are immediately available in the Group Policy Editor.

Go to the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise) to download the Microsoft Edge policy templates file (*MicrosoftEdgePolicyTemplates.cab*) and extract the contents.

#### Add the administrative template to Active Directory

1. On a domain controller or workstation with RSAT, browse to the **PolicyDefinition** folder (also known as the _Central Store_) on any domain controller for your domain. For older versions of Windows Server, you may need to create the PolicyDefinition folder. For more information, see [How to create and manage the Central Store for Group Policy Administrative Templates in Windows](https://support.microsoft.com/help/3087759/how-to-create-and-manage-the-central-store-for-group-policy-administra).
1. Open *MicrosoftEdgePolicyTemplates* and go to **windows** > **admx**.
1. Copy the *msedge.admx* file to the PolicyDefinition folder. (Example: %systemroot%\sysvol\domain\policies\PolicyDefinitions)
1. In the *admx* folder, open the appropriate language folder. For example, if you’re in the U.S., open the **en-US** folder.
1. Copy the *msedge.adml* file to the matching language folder in the PolicyDefinition folder. Create the folder if it does not already exist. (Example: %systemroot%\sysvol\domain\policies\PolicyDefinitions\EN-US)
1. If your domain has more than one domain controller, the new ADMX files will be replicated to them at the next domain replication interval.
1. To confirm the files loaded correctly, open the **Group Policy Management Editor** from Windows Administrative Tools and expand **Computer Configuration** > **Policies** > **Administrative Templates** > **Microsoft Edge**. You should see one or more Microsoft Edge nodes as shown below.

    ![Microsoft Edge policies](./media/configure-microsoft-edge/edge-gpo-policies.png)

#### Add the administrative template to an individual computer

1. On the target computer, open *MicrosoftEdgePolicyTemplates* and go to **windows** > **admx**.
2. Copy the *msedge.admx* file to your Policy Definition template folder. (Example: C:\Windows\PolicyDefinitions)
3. In the *admx* folder, open the appropriate language folder. For example, if you’re in the U.S., open the **en-US** folder.
4. Copy the *msedge.adml* file to the matching language folder in your Policy Definition folder. (Example: C:\Windows\PolicyDefinitions\en-US)
5. To confirm the files loaded correctly either open Local Group Policy Editor directly (Windows key + R and enter gpedit.msc) or open MMC and load the Local Group Policy Editor snap-in. If an error occurs, it’s usually because the files are in an incorrect location.

<!--
To add the administrative template to manage Microsoft Edge updates:

1. Open the *MicrosoftEdgePolicyTemplates* file and go to **windows** > **admx**.
2. Copy the *msedgeupdate.admx* file to your Policy Definition template folder. (Example: C:\Windows\PolicyDefinitions)
3. In the *updatepolicies* folder, open the appropriate language folder. For example, if you’re in Germany, open the **de-DE** folder.
4. Copy the *msedgeupdate.adml* file to the matching language folder in your Policy Definition folder. (Example: C:\Windows\PolicyDefinitions\de-DE)
5. Open MMC and load the Local Group Policy Editor snap-in to confirm the files loaded correctly. If an error occurs, it’s usually because the files are in an incorrect location.

> [!NOTE]
> Currently the Microsoft Edge update policies are only localized in en-US. Additional language support will be added in a future release.
-->

### 2. Set mandatory or recommended policies

You can set mandatory or recommended policies to configure Microsoft Edge with the Group Policy Editor for both Active Directory and individual computers. You can scope policy settings to either the **Computer Configuration** or **User Configuration** by selecting the appropriate node as described below.

- To configure a mandatory policy, open the Group Policy Editor and go to (**Computer Configuration** or **User Configuration**) > **Policies** > **Administrative Templates** > **Microsoft Edge**.
- To configure a recommended policy, open the Group Policy Editor and go to (**Computer Configuration** or **User Configuration**) > **Policies** > **Administrative Templates** > **Microsoft Edge – Default Settings (users can override)**.

  ![Open the Group Policy Editor](./media/configure-microsoft-edge/edge-ad-policy.png)

### 3. Test your policies

On a target client device, open Microsoft Edge and navigate to **edge://policy** to see all policies that are applied. If you applied policy settings on the local computer, policies should appear immediately. You may need to close and reopen Microsoft Edge if it was open while you were configuring policy settings.

![View configured policies in browser](./media/configure-microsoft-edge/edge-gpEdit.png)

For Active Directory group policy settings, policy settings are propagated to domain computers at a regular interval defined by your domain administrator, and target computers may not receive policy updates right away. To manually refresh Active Directory group policy settings on a target computer, execute the following command from a command prompt or PowerShell session on the target computer:

``` powershell
gpupdate /force
```

You may need to close and reopen Microsoft Edge before the new policies appear.

You can also use REGEDIT.exe on a target computer to view the registry settings that store group policy settings. These settings are located at the registry path **HKLM\SOFTWARE\Policies\Microsoft\Edge**.

## Frequently Asked Questions

### Can Microsoft Edge be configured to use master preferences?

Yes, you can configure Microsoft Edge to use a master preferences file.

 A master preferences file lets you configure default settings when Microsoft Edge is deployed. You can also use a master preferences file to apply settings on computers that aren't managed by a device management system. These settings are applied to the user’s profile the first time the user runs the browser. After the user runs the browser, changes to the master preferences file aren’t applied. A user can change settings from the master preferences in the browser. If you want to make a setting mandatory or change a setting after the first run of the browser, you must use a policy.

A master preferences file lets you to customize many different settings and preferences for the browser, including those shared with other Chromium based browsers and specific to Microsoft Edge.  Policy related preferences can be configured using the master preferences file. In cases where a policy is set and there’s a corresponding master preference set, the policy setting takes precedence.

> [!IMPORTANT]
> All the available preferences might not be consistent with Microsoft Edge terminology and naming conventions.  There’s no guarantee that these preferences will continue to work as expected in future releases. Preferences might be changed or ignored in later versions.

A master preferences file is a text file that’s formatted using JSON markup. This file needs to be added to the same directory as the msedge.exe executable. For system wide enterprise deployments on Windows this is typically: *Windows: C:\Program Files\Microsoft\Edge\Application\master_preferences*.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Configure for Windows with Intune](configure-edge-with-intune.md)
- [Configure for macOS](configure-microsoft-edge-on-mac.md)
- [Browse Microsoft Edge Enterprise Policies](microsoft-edge-policies.md)


