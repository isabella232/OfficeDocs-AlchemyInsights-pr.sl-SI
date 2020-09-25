---
title: 1490-odpravljanje težav-E-odkrivanje-napake
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277816"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="ff080-102">Odpravljanje napak pri iskanju vsebine</span><span class="sxs-lookup"><span data-stu-id="ff080-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="ff080-103">Ali imate težave z iskanjem vsebine ali pridobivanjem napak pri izvozu rezultatov iskanja?</span><span class="sxs-lookup"><span data-stu-id="ff080-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="ff080-104">Ali na primer prejemate te primere, ko izvajate iskanja?</span><span class="sxs-lookup"><span data-stu-id="ff080-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="ff080-105">Napake v CS008 ali CS012</span><span class="sxs-lookup"><span data-stu-id="ff080-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="ff080-106">Napake pri zasedenem strežniku/časovna omejitev</span><span class="sxs-lookup"><span data-stu-id="ff080-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="ff080-107">Prišlo je do napake pri programu</span><span class="sxs-lookup"><span data-stu-id="ff080-107">Application error occurred</span></span>

<span data-ttu-id="ff080-108">Ali pri iskanju ali izvozu rezultatov iz velikega števila nabiralnikov (prek nabiralnikov 100.000) prihaja do napak pri izvozu?</span><span class="sxs-lookup"><span data-stu-id="ff080-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="ff080-109">Za te vrste napak poskusite znova poiskati mesta vsebine, ki niso uspela.</span><span class="sxs-lookup"><span data-stu-id="ff080-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="ff080-110">Če želite več informacij, si oglejte  [Ta članek](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="ff080-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="ff080-111">Če izvažate več kot 100K nabiralnike, boste morali uporabiti ta PowerShell za prenos rezultatov izvoza:  [izvažanje rezultatov iz več kot 100k nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="ff080-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
