---
title: "Microsoft Edge Roadmap"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 01/15/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Roadmap"
---

# Microsoft Edge Roadmap

This article describes the roadmap for Microsoft Edge.

## Roadmap

| Description | Status | Tags | Release |
|--|--|--|--|
| Disallow synchronous XmlHttpRequest in page dismissal<br> <br> Sending of synchronous XmlHttpRequests during unload of a webpage will be removed. This change will improve browser performance and reliability, but may impact web applications that have not yet been updated to use more modern web APIs including sendBeacon and fetch.<br>Group Policy to disable this change and permit synchronous XHR during page dismissal will be available until Edge 88.<br> The current settings is behind a flag. Until enabled-by-default in Edge 82, this change can be previewed by setting edge://flags/#allow-sync-xhr-in-page-dismissal to Disabled.<br>[More information](https://docs.microsoft.com/microsoft-edge/web-platform/site-impacting-changes) | In development      |  Microsoft Edge, SAP    | Edge 82       |

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
