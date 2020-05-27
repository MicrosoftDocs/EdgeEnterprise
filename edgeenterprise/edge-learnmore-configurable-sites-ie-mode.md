---
title: "Microsoft Edge and configurable sites in IE mode"
ms.author: shisub
author: dan-wesley
manager: srugh
ms.date: 05/27/2020
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge and configurable sites in IE mode"
---

# Learn about configurable sites in IE mode

This article explains the Configurable Sites feature of the Enterprise Mode Site List when using IE mode in Microsoft Edge.

## Prerequisites

- Windows updates

  - Windows 10 version 1909, Windows server version 1909 – KB4550945  or higher
  - Windows 10 version 1903, Windows server version 1903 – KB4550945  or higher
  - Windows 10 version 1809, Windows Server version 1809, and Windows Server 2019 - KB4550969 or higher
  - Windows 10 version 1803 – KB4550944 or higher
  - Windows 10 version 1607, Windows Server 2016 - KB4556826 or higher
  - Windows 10 initial version, July 2015 - KB4550947 or higher
  - Windows 8.1 – KB4556798 or higher

- Microsoft Edge 82 (exact version) or later
- [IE mode](https://aka.ms/iemodeonedge) configured with Enterprise Mode Site List

## Overview

Configuring sites needing IE mode in the Enterprise Mode Site List will work well for most environments with legacy applications. However, in some cases this approach isn't the best to configure a subset of sites to open in IE mode without rendering an entire domain in IE mode. For example, when your environment contains both modern and legacy applications running on a single server and you would like the flexibility to render only the legacy applications in IE mode and the remaining applications to render in Microsoft Edge mode.

The solution is to use the Configurable Sites feature of the Enterprise Mode Site List. When the feature is enabled, the Microsoft Edge sitelist parser will allow sites with the "configurable" tag to participate in IE mode engine determination.

## How does it work?

### Automatic switching from Microsoft Edge to IE

To use the Configurable Sites feature, you'll need one or more sites in the Enterprise Mode Site List to have the `<open-in>Configurable</open-in>` option.

Example:

```
<site-list version="1">
  <site url="app.com">
    <open-in>Configurable</open-in>
  </site>
</site-list>
```

When the Configurable Sites feature is enabled, the following behavior occurs:

1. When making a request to a Configurable site, Microsoft Edge will send the HTTP request header "`X-InternetExplorerModeConfigurable: 1`".
2. A Configurable site may send a redirect response (for example, HTTP 302) with the HTTP response header "`X-InternetExplorerMode: 1`" to request that Microsoft Edge loads the site in IE mode.
3. The target of the redirect (that is, the value of the Location response header) must also be a Configurable or Neutral site, otherwise the IE mode response header will be ignored. It's expected that the target of the redirect will usually be the same as the original URL. However, it doesn't have to be.

   > [!NOTE]
   > The redirect response is subject to caching according to Microsoft Edge's normal HTTP caching behavior for redirects.

### Reverse switching from IE to Microsoft Edge

Enabling Configurable Sites in Microsoft Edge automatically enables the following behaviors in IE mode tabs:

1. When making a request to a Configurable site, IE mode tabs will send the HTTP request header "`X-InternetExplorerModeConfigurable: 1`", the same as Microsoft Edge tabs.
2. A Configurable site might send a redirect response (for example, HTTP 302) with the HTTP response header "`X-InternetExplorerMode: 0`" to request that the navigation switch back to Microsoft Edge mode (colloquially "reverse switching".)
3. The target of the redirect (that is, the value of the Location response header) must also be a Configurable or Neutral site, otherwise the IE mode response header will be ignored. It's expected that the target of the redirect will usually be the same as the original URL. However, it doesn't have to be.

   > [!NOTE]
   > The redirect response is subject to caching according to Microsoft Edge's normal HTTP caching behavior for redirects.

> [!TIP]
> Both browser engines send the same "`X-InternetExplorerModeConfigurable: 1`" request header to Configurable sites. You should use the User-Agent request header to distinguish between requests from Microsoft Edge mode vs. IE mode to avoid redirecting when the site is already loading in the correct engine.

## See also

- [About IE mode](https://docs.microsoft.com/deployedge/edge-ie-mode)
- [Additional Enterprise Mode information](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/enterprise-mode-overview-for-ie11)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)