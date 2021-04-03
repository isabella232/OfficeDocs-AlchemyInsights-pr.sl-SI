---
title: Razširitve za Google Chrome za Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505300"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="34182-102">Razširitve za Google Chrome za Microsoft Edge (Chromium)</span><span class="sxs-lookup"><span data-stu-id="34182-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="34182-103">Razširitve za [Google Chrome lahko preprosto odnehnete v brskalnik Microsoft Edge (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)</span><span class="sxs-lookup"><span data-stu-id="34182-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="34182-104">V večini primerov so za zagon teh razširitev v brskalniku Microsoft Edge potrebne le minimalne spremembe.</span><span class="sxs-lookup"><span data-stu-id="34182-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="34182-105">API-ji razširitve in ključi manifesta, ki jih podpira Google Chrome, so združljivi s kodo v brskalniku Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="34182-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="34182-106">Toda Microsoft Edge ne podpira razširitev API-jev chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken in chrome.instanceID.</span><span class="sxs-lookup"><span data-stu-id="34182-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>