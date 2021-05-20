---
title: Manjkajoča e-poštna sporočila v karanteni
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539840"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="61834-102">Manjkajoča e-poštna sporočila v karanteni«</span><span class="sxs-lookup"><span data-stu-id="61834-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="61834-103">Skrbniki si lahko [ogledajo ta sporočila, jih izdajajo ali izbrišejo.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="61834-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="61834-104">Če želite odpreti Središče & za skladnost s predpisi, odprite [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="61834-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="61834-105">Če želite stran Karantena odpreti neposredno, odprite [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="61834-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="61834-106">Iščete lahko po teh vrednostih:</span><span class="sxs-lookup"><span data-stu-id="61834-106">You can search by the following values:</span></span>  

- <span data-ttu-id="61834-107">**ID sporočila:** globalni enolični identifikator sporočila.</span><span class="sxs-lookup"><span data-stu-id="61834-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="61834-108">Če na seznamu izberete sporočilo, se vrednost  **ID-ja**  sporočila prikaže v  **prikazanem podoknu**  s podrobnostmi.</span><span class="sxs-lookup"><span data-stu-id="61834-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="61834-109">Skrbniki lahko s funkcijo [sledenja sporočilu](/microsoft-365/security/office-365-security/message-trace-scc) poiščejo sporočila in ustrezne vrednosti ID-ja sporočila.</span><span class="sxs-lookup"><span data-stu-id="61834-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="61834-110">**E-poštni naslov pošiljatelja:** e-poštni naslov enega pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="61834-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="61834-111">**E-poštni naslov** prejemnika: e-poštni naslov enega prejemnika.</span><span class="sxs-lookup"><span data-stu-id="61834-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="61834-112">**Zadeva:** uporabite celotno zadevo sporočila.</span><span class="sxs-lookup"><span data-stu-id="61834-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="61834-113">Iskanje ne uporablja velikih in malih črk.</span><span class="sxs-lookup"><span data-stu-id="61834-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="61834-114">Ko vnesete pogoje iskanja, kliknite Osveži gumb ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži, da** filtrirate rezultate.</span><span class="sxs-lookup"><span data-stu-id="61834-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="61834-115">Ukazi »cmdlet« za ogled in upravljanje sporočil in datotek v karanteni so:</span><span class="sxs-lookup"><span data-stu-id="61834-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="61834-116">Brisanje-karantenamessage</span><span class="sxs-lookup"><span data-stu-id="61834-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="61834-117">Izvoz v karanteno</span><span class="sxs-lookup"><span data-stu-id="61834-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="61834-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="61834-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="61834-119">[Predogled in pošiljanje sporočil v karanteni:](/powershell/module/exchange/preview-quarantinemessage)ta ukaz »cmdlet« je le za sporočila in ne za datoteke z zlonamerno programsko opremo iz programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive za podjetja ali Teams.</span><span class="sxs-lookup"><span data-stu-id="61834-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="61834-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="61834-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)