---
title: 1491 – iskanje – ne – vračanje – pričakovano – rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740490"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="bcafe-102">Iskanje po vsebini ne vrne pričakovanih rezultatov</span><span class="sxs-lookup"><span data-stu-id="bcafe-102">Content Search not returning expected results</span></span>

<span data-ttu-id="bcafe-103">Ko zaženete iskanje vsebine iz središča za preverjanje varnosti & za skladnost s predpisi Microsoft 365, lahko prejmete nepričakovane rezultate iskanja.</span><span class="sxs-lookup"><span data-stu-id="bcafe-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="bcafe-104">Razmislite o teh stvareh, ki lahko vplivajo na rezultate iskanja:</span><span class="sxs-lookup"><span data-stu-id="bcafe-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="bcafe-105">**Mesta vsebine in pogoji iskanja**: Preverite, ali ste izbrali ustrezna mesta vsebine in pogoje iskanja.</span><span class="sxs-lookup"><span data-stu-id="bcafe-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="bcafe-106">Če ste izvedli veliko iskanje (s številnimi lokacijami), jo razdelite na več iskanj.</span><span class="sxs-lookup"><span data-stu-id="bcafe-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="bcafe-107">**Delno indeksirani elementi**:  [delno indeksirani elementi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v ocenjene rezultate iskanja.</span><span class="sxs-lookup"><span data-stu-id="bcafe-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="bcafe-108">Vendar pa delno indeksirane elemente iz mest v SharePointu in OneDrive niso vključene v oceno iskanja.</span><span class="sxs-lookup"><span data-stu-id="bcafe-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="bcafe-109">**Napake pri iskanju**: pri iskanju velikega števila nabiralnikov (prek 100.000 nabiralnikov) lahko pride do napak pri iskanju, s kodami napak, kot so CS008-009 in CS012-002).</span><span class="sxs-lookup"><span data-stu-id="bcafe-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="bcafe-110">V tem primeru poskusite znova poiskati le neuspela mesta vsebine.</span><span class="sxs-lookup"><span data-stu-id="bcafe-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="bcafe-111">Če želite več informacij, si oglejte  [Ta članek](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="bcafe-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
