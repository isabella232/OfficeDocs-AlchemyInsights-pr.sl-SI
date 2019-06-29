---
title: Delo z iOS VPP aplikacije pravilo Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364883"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="85461-102">Delo z iOS aplikacije VPP</span><span class="sxs-lookup"><span data-stu-id="85461-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="85461-103">Preberite, [kako upravljati iOS aplikacije, kupljene prek obsega nakup program z Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) spoznajo značilnosti, omejitve in ukrepe, ki bodo uporabo Apple obsega nakup Program in podporo za to v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="85461-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="85461-104">**Pogosta vprašanja:** »Sem dodeljena iOS VPP app svojim uporabnikom, vendar namestitev ni uspela. «</span><span class="sxs-lookup"><span data-stu-id="85461-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="85461-105">To se lahko zgodi, če je čez več prenosen načrt upravljanja ponudniki enega žetona VPP.</span><span class="sxs-lookup"><span data-stu-id="85461-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="85461-106">VPP žetonov iz Apple se lahko uporabijo le pri enem ponudniku.</span><span class="sxs-lookup"><span data-stu-id="85461-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="85461-107">Če ste uporabili VPP žeton z več ponudniki, mora ponovno naložite žeton za Intune.</span><span class="sxs-lookup"><span data-stu-id="85461-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="85461-108">Namestitev lahko tudi ne, če je skupno število naprav presega število licenc.</span><span class="sxs-lookup"><span data-stu-id="85461-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="85461-109">Ogledati navada referat za licence, pojdite na **Intune prenosen apps** \> **App licence** strani.</span><span class="sxs-lookup"><span data-stu-id="85461-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="85461-110">Če želite izvedeti kako do povračila dovoljenja v uporabi, glejte [Ta članek.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="85461-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
