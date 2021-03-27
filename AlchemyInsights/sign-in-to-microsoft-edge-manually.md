---
title: Ročni vpis v Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398673"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="2d967-102">Ročni vpis v Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2d967-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="2d967-103">Če se uporabnik med izkušnjo prvega zagona ne vpiše samodejno, se lahko uporabnik ročno vpiše v nastavitvah brskalnika ali v letaku za identiteto.</span><span class="sxs-lookup"><span data-stu-id="2d967-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="2d967-104">Če želite upravljati vpis, uporabite te pravilnike:</span><span class="sxs-lookup"><span data-stu-id="2d967-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="2d967-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – če želite zagotoviti, da ima uporabnik vedno službeni profil v brskalniku Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="2d967-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="2d967-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – Če želite omejiti vpis v nabor zaupanja vrednih računov.</span><span class="sxs-lookup"><span data-stu-id="2d967-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="2d967-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – če želite onemogočiti vpis ali prisiliti uporabnike, da se vpišejo.</span><span class="sxs-lookup"><span data-stu-id="2d967-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

