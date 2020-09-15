---
title: AntiSpam 5.4.1 DBEB Catch-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717377"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="58db8-102">Odpravljanje težav z dostavo za kodo napake 550 za dostop do posredovanja</span><span class="sxs-lookup"><span data-stu-id="58db8-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="58db8-103">Do te težave pride pri [preverjanju, ali je e-poštni naslov veljaven, da preprečite bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri vnosu Microsoftovega omrežja.</span><span class="sxs-lookup"><span data-stu-id="58db8-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="58db8-104">Preskusite to:</span><span class="sxs-lookup"><span data-stu-id="58db8-104">Try the following:</span></span>

1. <span data-ttu-id="58db8-105">Določite, ali je težava značilna za celotno domeno ali en e-poštni naslov:</span><span class="sxs-lookup"><span data-stu-id="58db8-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="58db8-106">Celotna domena: včasih je treba domeno sinhronizirati; poskusite [nastaviti domeno na notranjo in nato spet na avtoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="58db8-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="58db8-107">En e-poštni naslov: včasih je treba naslov sinhronizirati; Če želite spremeniti naslov strežnika proxy SMTP in ga nato znova spremeniti, lahko pomagate.</span><span class="sxs-lookup"><span data-stu-id="58db8-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="58db8-108">Določite, ali je težava značilna za skupino ali javno mapo.</span><span class="sxs-lookup"><span data-stu-id="58db8-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="58db8-109">Za nekatere vrste predmetov morajo biti predmeti morda ročno ustvarjeni v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="58db8-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="58db8-110">Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, ki ga pošiljate), tako da vam lahko pomagamo bolje.</span><span class="sxs-lookup"><span data-stu-id="58db8-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>