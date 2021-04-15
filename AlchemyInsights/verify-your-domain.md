---
title: Preverjanje domene
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771007"
---
# <a name="verify-your-domain"></a><span data-ttu-id="1ef64-102">Preverjanje domene</span><span class="sxs-lookup"><span data-stu-id="1ef64-102">Verify your domain</span></span>

 <span data-ttu-id="1ef64-103">**Zapis verjetno ni bil posodobljen v internetu.**</span><span class="sxs-lookup"><span data-stu-id="1ef64-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="1ef64-104">Običajno traja le nekaj minut, da si lahko ogledamo nov zapis, občasno pa lahko traja tudi nekaj ur.</span><span class="sxs-lookup"><span data-stu-id="1ef64-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="1ef64-105">Če ste čakali že tako dolgo, še enkrat preverite, ali ste kopirali in prilepili natančno vrednost v zapis preverjanja TXT pri gostitelju zapisov DNS.</span><span class="sxs-lookup"><span data-stu-id="1ef64-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="1ef64-106">Ena pogosta težava je, da ni 4 dela zapisa »MS=«.</span><span class="sxs-lookup"><span data-stu-id="1ef64-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="1ef64-107">Tudi to potrebujemo!</span><span class="sxs-lookup"><span data-stu-id="1ef64-107">We need that too!</span></span>

- <span data-ttu-id="1ef64-108">Pri nekaterih gostiteljih zapisov DNS morate še dodatno shraniti datoteko območja (kjer je zapis DNS shranjen), tako da se bo posodobil v internetu.</span><span class="sxs-lookup"><span data-stu-id="1ef64-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="1ef64-109">Shranite spremembe, da bo Microsoft lahko videl in preveril zapis.</span><span class="sxs-lookup"><span data-stu-id="1ef64-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
