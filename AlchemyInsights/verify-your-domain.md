---
title: Preverjanje domene
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365433"
---
# <a name="verify-your-domain"></a><span data-ttu-id="2ae16-102">Preverjanje domene</span><span class="sxs-lookup"><span data-stu-id="2ae16-102">Verify your domain</span></span>

 <span data-ttu-id="2ae16-103">**Zapis verjetno ni posodobljen prek interneta.**</span><span class="sxs-lookup"><span data-stu-id="2ae16-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="2ae16-104">To običajno traja le nekaj minut za nas, da lahko videli nov zapis, vendar občasno lahko traja tako dolgo, kot nekaj ur.</span><span class="sxs-lookup"><span data-stu-id="2ae16-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="2ae16-105">Če ste čakali tako dolgo že, še enkrat preverite, da ste kopirali in prilepili natančna vrednost v zapisu TXT preverjanje na vaš DNS strežnik.</span><span class="sxs-lookup"><span data-stu-id="2ae16-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="2ae16-106">Eno skupno težavo ne vključuje v "MS =" del zapisa.</span><span class="sxs-lookup"><span data-stu-id="2ae16-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="2ae16-107">Moramo, da preveč!</span><span class="sxs-lookup"><span data-stu-id="2ae16-107">We need that too!</span></span>

- <span data-ttu-id="2ae16-108">Na nekaterih DNS gostiteljev, moraš sprejeti dodaten korak, da shranite pas (kjer DNS zapis se shrani) tako, da bo posodobitev prek interneta.</span><span class="sxs-lookup"><span data-stu-id="2ae16-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="2ae16-109">Preverite, ali ste shranili spremembe tako Office 365 lahko videli in preverjanje zapisa.</span><span class="sxs-lookup"><span data-stu-id="2ae16-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
