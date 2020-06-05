---
title: Manjkajoče e-pošte v karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569560"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="2dcd5-102">Manjkajoče e-pošte v karanteni "</span><span class="sxs-lookup"><span data-stu-id="2dcd5-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="2dcd5-103">Skrbniki [si lahko ta sporočila ogledajo, sprostijo ali izbrišejo.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2dcd5-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="2dcd5-104">Če želite odpreti središče za skladnost varnostnega &, pojdite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="2dcd5-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="2dcd5-105">Če želite neposredno odpreti stran» karantena «, pojdite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="2dcd5-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="2dcd5-106">Iščete lahko po naslednjih vrednostih:</span><span class="sxs-lookup"><span data-stu-id="2dcd5-106">You can search by the following values:</span></span>  

- <span data-ttu-id="2dcd5-107">**ID sporočila**: globalni enolični identifikator sporočila.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="2dcd5-108">Če na seznamu izberete sporočilo, se vrednost ID- **ja sporočila** prikaže v podoknu za Pojavni meni **podrobnosti** , ki se prikaže.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="2dcd5-109">Skrbniki lahko s [sledenjem sporočilom](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najdejo sporočila in ustrezne vrednosti ID-ja sporočila.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="2dcd5-110">**E-poštni naslov pošiljatelja**: e-poštni naslov enega pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="2dcd5-111">**E-poštni naslov prejemnika**: e-poštni naslov enega prejemnika.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="2dcd5-112">**Zadeva**: uporabite celoten predmet sporočila.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="2dcd5-113">Iskanje ni občutljivo na male črke.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="2dcd5-114">Ko vnesete kriterije iskanja, kliknite Osveži ![ gumb ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži** , da filtrirate rezultate.  </span><span class="sxs-lookup"><span data-stu-id="2dcd5-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="2dcd5-115">Ukazi» cmdlet «, ki jih uporabljate za ogled in upravljanje sporočil in datotek v karanteni, so:</span><span class="sxs-lookup"><span data-stu-id="2dcd5-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="2dcd5-116">Izbriši-karantenski sporočilo</span><span class="sxs-lookup"><span data-stu-id="2dcd5-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="2dcd5-117">Sporočilo za izvoz-karanteno</span><span class="sxs-lookup"><span data-stu-id="2dcd5-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="2dcd5-118">Sporočilo v karanteni</span><span class="sxs-lookup"><span data-stu-id="2dcd5-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="2dcd5-119">[Predogled-v karanteni](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Upoštevajte, da je ta ukaz» cmdlet «samo za sporočila, ne pa zlonamerna datoteka iz ATP za SharePoint online, OneDrive za podjetja ali ekipe.</span><span class="sxs-lookup"><span data-stu-id="2dcd5-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="2dcd5-120">Sporočilo za sprostitev-karanteno</span><span class="sxs-lookup"><span data-stu-id="2dcd5-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)