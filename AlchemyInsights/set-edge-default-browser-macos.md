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
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="46eac-102">Nastavitev brskalnika Microsoft Edge kot privzetega brskalnika v napravi s sistemom macOS</span><span class="sxs-lookup"><span data-stu-id="46eac-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="46eac-103">Microsoft Edge nastavite kot privzeti brskalnik na enega od teh dveh načinov:</span><span class="sxs-lookup"><span data-stu-id="46eac-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="46eac-104">1. način: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span><span class="sxs-lookup"><span data-stu-id="46eac-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="46eac-105">2. način: Nastavite pravilnik DefaultBrowserSettingEnabled, da uporabnika pozove, da nastavi Microsoft Edge kot privzeti brskalnik.</span><span class="sxs-lookup"><span data-stu-id="46eac-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="46eac-106">Na kateri koli način lahko uporabnik spremeni privzeti brskalnik.</span><span class="sxs-lookup"><span data-stu-id="46eac-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="46eac-107">Zato vam priporočamo, da uvedete pravilnik DefaultBrowserSettingEnabled, tudi če ste uporabili 1. način.</span><span class="sxs-lookup"><span data-stu-id="46eac-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="46eac-108">Če uporabnik po uvedenem pravilniku spremeni privzeti brskalnik, ga pravilnik pozove, da privzeti brskalnik nastavi nazaj na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="46eac-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
