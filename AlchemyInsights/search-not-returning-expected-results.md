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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776097"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="22854-102">Vsebino iskanje ne vrne pričakovanih rezultatov</span><span class="sxs-lookup"><span data-stu-id="22854-102">Content Search not returning expected results</span></span>

<span data-ttu-id="22854-103">Ko teče vsebine iskanja iz Office 365 varnostno & Center skladnosti, se lahko prikaže nepričakovano zadetkov.</span><span class="sxs-lookup"><span data-stu-id="22854-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="22854-104">Razmislite o naslednjih stvari, ki lahko vplivajo na rezultate iskanja:</span><span class="sxs-lookup"><span data-stu-id="22854-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="22854-105">**Vsebine mesta in iskalne pogoje**: poskrbite, da boste izbrali ustrezno vsebine mesta in iskalne pogoje.</span><span class="sxs-lookup"><span data-stu-id="22854-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="22854-106">Če ste zagnali veliko iskanje (z veliko lokacij), menijo, da razdelite v več iskanj.</span><span class="sxs-lookup"><span data-stu-id="22854-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="22854-107">**Delno indeksirane postavke**: [delno indeksirane postavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v rezultatih ocenjena.</span><span class="sxs-lookup"><span data-stu-id="22854-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="22854-108">Vendar, delno indeksiranih elementi iz mesta in SharePoint OneDrive niso vključeni v oceni Išči.</span><span class="sxs-lookup"><span data-stu-id="22854-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="22854-109">**Iskanje napak**: pri iskanju veliko število nabiralnikov (več kot 100.000 nabiralnikov), lahko dobite iskanje napak, s zmota zbornik CS008-009 in CS012-002).</span><span class="sxs-lookup"><span data-stu-id="22854-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="22854-110">V tem primeru ponovite iskanje le ni vsebine mesta.</span><span class="sxs-lookup"><span data-stu-id="22854-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="22854-111">Glej [Ta članek](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="22854-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
