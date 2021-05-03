---
title: Odpravljanje težav z obtičim opravilom uvoza storitve
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125494"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="019f9-102">Odpravljanje težav z obtičim opravilom uvoza storitve</span><span class="sxs-lookup"><span data-stu-id="019f9-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="019f9-103">Če prihaja do težav z obtičim ali neuspešnim uvozom storitve, preglejte in poskusite to:</span><span class="sxs-lookup"><span data-stu-id="019f9-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="019f9-104">Preglejte velikost datoteke PST.</span><span class="sxs-lookup"><span data-stu-id="019f9-104">Review the size of of the PST file.</span></span> <span data-ttu-id="019f9-105">Največja priporočena velikost datoteke PST za uvoz je 20 GB.</span><span class="sxs-lookup"><span data-stu-id="019f9-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="019f9-106">Če sumite, da so preskočeni elementi zaradi poškodbe, zaženite Scanpst.exe, da diagnosticirate in odpravite napake v datotekah PST.</span><span class="sxs-lookup"><span data-stu-id="019f9-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="019f9-107">Če se med uvozom prikaže napaka »MapiExceptionShutoffQuotaExceeded«, preverite, ali je ciljni nabiralnik dovolj zmogljivosti za uvoz želenih datotek PST.</span><span class="sxs-lookup"><span data-stu-id="019f9-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="019f9-108">Če želite več informacij o odpravljanju težav z uvozom datotek PST, glejte [Odpravljanje težav z posli uvoza datotek PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="019f9-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="019f9-109">Če želite informacije o tem, kako odpravite težave pri uvozu datotek PSTs v Outlook, glejte Odpravljanje težav pri uvozu [datoteke .pst (microsoft.com Outlook ).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="019f9-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>