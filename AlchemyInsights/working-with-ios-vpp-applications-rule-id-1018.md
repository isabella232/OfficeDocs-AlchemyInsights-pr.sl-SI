---
title: Delo z iOS VPP aplikacije pravilo ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719973"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="cf0dd-102">Delo z iOS VPP aplikacije</span><span class="sxs-lookup"><span data-stu-id="cf0dd-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="cf0dd-103">Preberite, [Kako upravljate aplikacije za iOS, kupljene prek programa za nakup nosilcev z Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) , če želite izvedeti več o funkcijah, omejitvah in korakih za uporabo programa Apple Volume nakup in podporo za to v Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="cf0dd-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="cf0dd-104">**Pogosta vprašanja:** » Za svoje uporabnike sem dodelil aplikacijo iOS VPP, vendar namestitev ni uspela. «</span><span class="sxs-lookup"><span data-stu-id="cf0dd-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="cf0dd-105">To se lahko zgodi, če je uporabljen en žeton VPP v več ponudnikih upravljanja mobilnih naprav.</span><span class="sxs-lookup"><span data-stu-id="cf0dd-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="cf0dd-106">Žetoni VPP iz Apple se lahko uporabljajo samo z enim ponudnikom.</span><span class="sxs-lookup"><span data-stu-id="cf0dd-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="cf0dd-107">Če ste žeton VPP uporabili z več ponudniki, morate žeton znova naložiti v InTune.</span><span class="sxs-lookup"><span data-stu-id="cf0dd-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="cf0dd-108">Namestitev lahko spodleti tudi, če skupno število naprav preseže število licenc.</span><span class="sxs-lookup"><span data-stu-id="cf0dd-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="cf0dd-109">Če si želite ogledati poročilo o uporabi za licence, pojdite na stran z \> **licencami** za **aplikacije za mobilne naprave** .</span><span class="sxs-lookup"><span data-stu-id="cf0dd-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="cf0dd-110">Če želite izvedeti, kako znova pridobiti licence v uporabi, si oglejte [Ta članek.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="cf0dd-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
