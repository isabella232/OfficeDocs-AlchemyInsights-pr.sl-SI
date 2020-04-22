---
title: 1491-iskanje-ne vrača-pričakovani-rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709243"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="9f53f-102">Iskanje vsebine ne vrača pričakovanih rezultatov</span><span class="sxs-lookup"><span data-stu-id="9f53f-102">Content Search not returning expected results</span></span>

<span data-ttu-id="9f53f-103">Ko izvajate iskanja po vsebini iz Microsoft 365 Security & center za skladnost, lahko prejmete nepričakovane rezultate iskanja.</span><span class="sxs-lookup"><span data-stu-id="9f53f-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="9f53f-104">Razmislite o naslednjih stvareh, ki lahko vplivajo na rezultate iskanja:</span><span class="sxs-lookup"><span data-stu-id="9f53f-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="9f53f-105">**Mesta vsebine in pogoji iskanja**: Prepričajte se, da ste izbrali ustrezne lokacije vsebine in iskalne pogoje.</span><span class="sxs-lookup"><span data-stu-id="9f53f-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="9f53f-106">Če ste zagnali veliko iskanje (z mnogimi lokacijami), razmislite o razdelitvi v več iskanj.</span><span class="sxs-lookup"><span data-stu-id="9f53f-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="9f53f-107">**Delno indeksirani elementi**: [delno indeksirani elementi](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v ocenjene rezultate iskanja.</span><span class="sxs-lookup"><span data-stu-id="9f53f-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="9f53f-108">Vendar pa delno indeksirani elementi iz mest v SharePointu in storitvi OneDrive niso vključeni v oceno iskanja.</span><span class="sxs-lookup"><span data-stu-id="9f53f-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="9f53f-109">**Napake pri iskanju**: pri iskanju velikega števila nabiralnikov (več kot 100.000 nabiralnikov) lahko dobite napake pri iskanju, s kodami napak, kot sta CS008-009 in CS012-002).</span><span class="sxs-lookup"><span data-stu-id="9f53f-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="9f53f-110">V tem primeru poskusite znova iskati samo za neuspele lokacije vsebine.</span><span class="sxs-lookup"><span data-stu-id="9f53f-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="9f53f-111">Za več informacij glejte [Ta članek](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="9f53f-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
