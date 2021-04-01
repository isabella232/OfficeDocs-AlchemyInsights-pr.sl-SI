---
title: Nastavitev brskalnika Microsoft Edge kot privzetega brskalnika v napravi s sistemom macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491815"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Nastavitev brskalnika Microsoft Edge kot privzetega brskalnika v napravi s sistemom macOS

Microsoft Edge nastavite kot privzeti brskalnik na enega od teh dveh načinov:

1. način: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.

2. način: Nastavite pravilnik DefaultBrowserSettingEnabled, da uporabnika pozove, da nastavi Microsoft Edge kot privzeti brskalnik.

Na kateri koli način lahko uporabnik spremeni privzeti brskalnik. Zato vam priporočamo, da uvedete pravilnik DefaultBrowserSettingEnabled, tudi če ste uporabili 1. način. Če uporabnik po uvedenem pravilniku spremeni privzeti brskalnik, ga pravilnik pozove, da privzeti brskalnik nastavi nazaj na Microsoft Edge.
