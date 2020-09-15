---
title: Delo s pravilnikom za VPP aplikacije iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688962"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="74106-102">Delo z aplikacijami iOS VPP</span><span class="sxs-lookup"><span data-stu-id="74106-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="74106-103">Preberite, [Kako upravljate aplikacije iOS, kupljene prek programa za nakup zvezka, z aplikacijo Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) , če želite izvedeti več o funkcijah, omejitvah in korakih za uporabo programa Apple za nakup količin in podpore za Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="74106-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="74106-104">**Pogoste težave:** » Uporabnikom sem dodelil program iOS VPP, vendar namestitev ni uspela. «</span><span class="sxs-lookup"><span data-stu-id="74106-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="74106-105">Do tega lahko pride, če je en žeton VPP uporabljen v več ponudnikih za upravljanje mobilnih naprav.</span><span class="sxs-lookup"><span data-stu-id="74106-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="74106-106">VPP žetoni iz Apple se lahko uporabljajo le z enim ponudnikom.</span><span class="sxs-lookup"><span data-stu-id="74106-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="74106-107">Če ste uporabili žeton» VPP «z več ponudniki, morate znova prenesti žeton na InTune.</span><span class="sxs-lookup"><span data-stu-id="74106-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="74106-108">Namestitev lahko tudi ne uspe, če skupno število naprav preseže število licenc.</span><span class="sxs-lookup"><span data-stu-id="74106-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="74106-109">Če si želite ogledati poročilo o uporabi za svoje licence, pojdite **Intune Mobile apps** na stran z \> **licencami** za InTune aplikacije Mobile.</span><span class="sxs-lookup"><span data-stu-id="74106-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="74106-110">Če želite izvedeti več o potrditvi licenc v uporabi, si oglejte [Ta članek.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="74106-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
