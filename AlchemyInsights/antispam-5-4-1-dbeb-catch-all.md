---
title: AntiSpam 5.4.1 DBEB Catch-vse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707927"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="5524b-102">Fix dostava vprašanja za kodo napake 550 5.4.1 Relay dostop zavrnjen</span><span class="sxs-lookup"><span data-stu-id="5524b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="5524b-103">Do te težave pride, ko [preverjate, ali je e-poštni naslov veljaven za preprečitev odskakanja](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ob vstopu v Microsoftovo omrežje.</span><span class="sxs-lookup"><span data-stu-id="5524b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="5524b-104">Poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="5524b-104">Try the following:</span></span>

1. <span data-ttu-id="5524b-105">Ugotovite, ali je težava specifična za celotno domeno ali en sam e-poštni naslov:</span><span class="sxs-lookup"><span data-stu-id="5524b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="5524b-106">Celotna domena: včasih domeno je treba sinhronizirati; začeti [postavljanje področje v notranji ter torej prislon v verodostojni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="5524b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="5524b-107">En e-poštni naslov: včasih je treba naslov sinhronizirati; Spreminjanje naslova strežnika SMTP in ga nato spremeni nazaj, lahko pomaga.</span><span class="sxs-lookup"><span data-stu-id="5524b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="5524b-108">Ugotovite, ali je težava specifična za skupino ali javno mapo.</span><span class="sxs-lookup"><span data-stu-id="5524b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="5524b-109">Za nekatere vrste predmetov bo morda treba predmete ročno ustvariti v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5524b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="5524b-110">Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, ki ga pošiljate), da vam lahko pomagamo bolje.</span><span class="sxs-lookup"><span data-stu-id="5524b-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>