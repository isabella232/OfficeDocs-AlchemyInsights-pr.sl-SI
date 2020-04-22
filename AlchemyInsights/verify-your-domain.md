---
title: Preverjanje domene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710459"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a2289-102">Preverjanje domene</span><span class="sxs-lookup"><span data-stu-id="a2289-102">Verify your domain</span></span>

 <span data-ttu-id="a2289-103">**Zapis verjetno ni posodobljen preko interneta.**</span><span class="sxs-lookup"><span data-stu-id="a2289-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a2289-104">To običajno traja le nekaj minut, da bomo lahko videli nov zapis, vendar občasno lahko traja tako dolgo, kot nekaj ur.</span><span class="sxs-lookup"><span data-stu-id="a2289-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a2289-105">Če ste že dolgo čakali na to, dvakrat preverite, ali ste kopirali in prilepili natančno vrednost v zapis preverjanja TXT pri gostitelju DNS.</span><span class="sxs-lookup"><span data-stu-id="a2289-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a2289-106">Eno skupno vprašanje ne vključuje "MS =" del zapisa.</span><span class="sxs-lookup"><span data-stu-id="a2289-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a2289-107">Tudi to potrebujemo!</span><span class="sxs-lookup"><span data-stu-id="a2289-107">We need that too!</span></span>

- <span data-ttu-id="a2289-108">Pri nekaterih DNS gostiteljih morate sprejeti dodaten korak, da shranite datoteko cone (kjer je shranjen zapis DNS), tako da bo posodobljen po internetu.</span><span class="sxs-lookup"><span data-stu-id="a2289-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a2289-109">Poskrbite, da ste shranili spremembe, da bo Microsoft lahko videl in preveril zapis.</span><span class="sxs-lookup"><span data-stu-id="a2289-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
