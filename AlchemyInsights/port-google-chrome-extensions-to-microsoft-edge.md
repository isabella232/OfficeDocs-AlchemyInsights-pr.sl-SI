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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Razširitve za Google Chrome za Microsoft Edge (Chromium)

Razširitve za [Google Chrome lahko preprosto odnehnete v brskalnik Microsoft Edge (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) V večini primerov so za zagon teh razširitev v brskalniku Microsoft Edge potrebne le minimalne spremembe.

API-ji razširitve in ključi manifesta, ki jih podpira Google Chrome, so združljivi s kodo v brskalniku Microsoft Edge. Toda Microsoft Edge ne podpira razširitev API-jev chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken in chrome.instanceID.