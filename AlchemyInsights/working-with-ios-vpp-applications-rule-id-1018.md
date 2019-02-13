---
title: Delo z iOS VPP aplikacije pravilo Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917512"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="48633-102">Delo z iOS aplikacije VPP</span><span class="sxs-lookup"><span data-stu-id="48633-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="48633-103">Preberite, [kako upravljati iOS aplikacije, kupljene prek obsega nakup program z Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) spoznajo značilnosti, omejitve in ukrepe, ki bodo uporabo Apple obsega nakup Program in podporo za to v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="48633-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="48633-104">**Pogosta vprašanja:** »Sem dodeljena iOS VPP app svojim uporabnikom, vendar namestitev ni uspela. «</span><span class="sxs-lookup"><span data-stu-id="48633-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="48633-p101">To se lahko zgodi, če je čez več prenosen načrt upravljanja ponudniki enega žetona VPP. VPP žetonov iz Apple se lahko uporabijo le pri enem ponudniku. Če ste uporabili VPP žeton z več ponudniki, mora ponovno naložite žeton za Intune.</span><span class="sxs-lookup"><span data-stu-id="48633-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="48633-p102">Namestitev lahko tudi ne, če je skupno število naprav presega število licenc. Ogledati navada referat za licence, pojdite na **Intune prenosen apps** \> **App licence** strani. Če želite izvedeti kako do povračila dovoljenja v uporabi, glejte [Ta članek.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="48633-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

