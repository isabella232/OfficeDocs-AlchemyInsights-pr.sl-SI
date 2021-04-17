---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821463"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="be1c3-102">Odpravljanje težav z dostavo kode napake 550 5.4.1 zavrnjen dostop do posredovalnega strežnika</span><span class="sxs-lookup"><span data-stu-id="be1c3-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="be1c3-103">Do te težave pride pri preverjanju, ali je e-poštni naslov veljaven in preprečuje povratne podatke o [odklonih, ko](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) vnašate podatke v Microsoftovo omrežje.</span><span class="sxs-lookup"><span data-stu-id="be1c3-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="be1c3-104">Poskusite to:</span><span class="sxs-lookup"><span data-stu-id="be1c3-104">Try the following:</span></span>

1. <span data-ttu-id="be1c3-105">Določite, ali je težava specifična za celotno domeno ali en e-poštni naslov:</span><span class="sxs-lookup"><span data-stu-id="be1c3-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="be1c3-106">Celotna domena: včasih je treba domeno sinhronizirati; poskusite [nastaviti domeno na Notranje in nato nazaj na Avtoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="be1c3-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="be1c3-107">En e-poštni naslov: včasih je treba naslov sinhronizirati; lahko pomagate tako, da spremenite naslov proxy smtp in ga nato znova spremenite.</span><span class="sxs-lookup"><span data-stu-id="be1c3-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="be1c3-108">Določite, ali je težava specifična za skupino ali javno mapo.</span><span class="sxs-lookup"><span data-stu-id="be1c3-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="be1c3-109">Za nekatere vrste predmetov boste morda morali predmete ustvariti ročno v imeniku Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="be1c3-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="be1c3-110">Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, na katere pošiljate), da vam bomo lahko pomagali bolje.</span><span class="sxs-lookup"><span data-stu-id="be1c3-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>