---
title: Manjkajoča e-poštna sporočila v karanteni
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673730"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="a5ec8-102">Manjkajoča e-poštna sporočila v karanteni</span><span class="sxs-lookup"><span data-stu-id="a5ec8-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="a5ec8-103">Skrbniki [si lahko ogledajo, izdajajo ali izbrišejo ta sporočila.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a5ec8-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="a5ec8-104">Če želite odpreti središče za skladnost varnostnega &, pojdite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="a5ec8-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="a5ec8-105">Če želite odpreti stran karantene neposredno, pojdite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="a5ec8-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="a5ec8-106">Iščete lahko po teh vrednostih:</span><span class="sxs-lookup"><span data-stu-id="a5ec8-106">You can search by the following values:</span></span>  

- <span data-ttu-id="a5ec8-107">**ID sporočila**: globalni enolični identifikator sporočila.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="a5ec8-108">Če izberete sporočilo na seznamu, se prikaže vrednost  **ID sporočila**  v podoknu  **podrobnosti**  flyout, ki se prikaže.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="a5ec8-109">Skrbniki lahko s [sledenjem sporočil](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) poiščejo sporočila in njihove ustrezne vrednosti ID-ja sporočila.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="a5ec8-110">**Pošiljatelj e-poštni naslov**: e-poštni naslov enega pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="a5ec8-111">**E-poštni naslov prejemnika**: e-poštni naslov posameznega prejemnika.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="a5ec8-112">**Zadeva**: uporabite celotno zadevo sporočila.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="a5ec8-113">Iskanje ne razlikuje med velikimi in malimi črkami.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="a5ec8-114">Ko vnesete pogoje iskanja, kliknite Osveži gumb Osveži, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** da filtrirate rezultate.  </span><span class="sxs-lookup"><span data-stu-id="a5ec8-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="a5ec8-115">Ukazi» cmdlet «, ki jih uporabljate za ogled in upravljanje sporočil in datotek v karanteni, so:</span><span class="sxs-lookup"><span data-stu-id="a5ec8-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="a5ec8-116">Izbriši-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a5ec8-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="a5ec8-117">Izvoz – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a5ec8-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="a5ec8-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a5ec8-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="a5ec8-119">[Predogled – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Upoštevajte, da je ta ukaz» cmdlet «le za sporočila in ne zlonamerne programske opreme v storitvi ATP za SharePoint online, OneDrive za podjetja ali teams.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="a5ec8-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a5ec8-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)