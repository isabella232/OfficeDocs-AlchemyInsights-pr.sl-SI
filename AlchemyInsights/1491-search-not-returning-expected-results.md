---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964965"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="c3fa4-102">Vsebino iskanje ne vrne pričakovanih rezultatov</span><span class="sxs-lookup"><span data-stu-id="c3fa4-102">Content Search not returning expected results</span></span>

<span data-ttu-id="c3fa4-p101">Ko teče vsebine iskanja iz Office 365 varnostno & Center skladnosti, se lahko prikaže nepričakovano zadetkov. Razmislite o naslednjih stvari, ki lahko vplivajo na rezultate iskanja:</span><span class="sxs-lookup"><span data-stu-id="c3fa4-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="c3fa4-p102">**Vsebine mesta in iskalne pogoje**: poskrbite, da boste izbrali ustrezno vsebine mesta in iskalne pogoje. Če ste zagnali veliko iskanje (z veliko lokacij), menijo, da razdelite v več iskanj.</span><span class="sxs-lookup"><span data-stu-id="c3fa4-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="c3fa4-p103">**Delno indeksirane postavke**: [delno indeksirane postavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v rezultatih ocenjena. Vendar, delno indeksiranih elementi iz mesta in SharePoint OneDrive niso vključeni v oceni Išči.</span><span class="sxs-lookup"><span data-stu-id="c3fa4-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="c3fa4-p104">**Iskanje napak**: pri iskanju veliko število nabiralnikov (več kot 100.000 nabiralnikov), lahko dobite iskanje napak, s zmota zbornik CS008-009 in CS012-002). V tem primeru ponovite iskanje le ni vsebine mesta. Glej [Ta članek](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="c3fa4-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
