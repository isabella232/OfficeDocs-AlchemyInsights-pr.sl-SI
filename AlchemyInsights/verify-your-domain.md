---
title: Preverjanje domene
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734322"
---
# <a name="verify-your-domain"></a><span data-ttu-id="b4cf1-102">Preverjanje domene</span><span class="sxs-lookup"><span data-stu-id="b4cf1-102">Verify your domain</span></span>

 <span data-ttu-id="b4cf1-103">**Zapis verjetno ni bil posodobljen prek interneta.**</span><span class="sxs-lookup"><span data-stu-id="b4cf1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="b4cf1-104">Po navadi traja le nekaj minut, da si lahko ogledate nov zapis, občasno pa lahko traja le nekaj ur.</span><span class="sxs-lookup"><span data-stu-id="b4cf1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="b4cf1-105">Če ste že dolgo čakali, dvakrat preverite, ali ste kopirali in prilepili natančno vrednost v zapis za preverjanje TXT pri gostitelju DNS.</span><span class="sxs-lookup"><span data-stu-id="b4cf1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="b4cf1-106">Ena pogosta težava ni vključena v del zapisa» MS = «.</span><span class="sxs-lookup"><span data-stu-id="b4cf1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="b4cf1-107">Tudi to potrebujemo!</span><span class="sxs-lookup"><span data-stu-id="b4cf1-107">We need that too!</span></span>

- <span data-ttu-id="b4cf1-108">Pri nekaterih gostiteljih DNS morate dodatno ukrepati, če želite shraniti datoteko območja (kjer je zapis DNS shranjen), tako da se bo posodobil prek interneta.</span><span class="sxs-lookup"><span data-stu-id="b4cf1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="b4cf1-109">Prepričajte se, da ste shranili spremembe, tako da lahko Microsoft vidi in preveri zapis.</span><span class="sxs-lookup"><span data-stu-id="b4cf1-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
