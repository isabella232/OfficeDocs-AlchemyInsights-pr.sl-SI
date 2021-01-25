---
title: Nabiralnik v arhivu je skoraj poln
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974664"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="fe9e0-102">Nabiralnik v arhivu je skoraj poln</span><span class="sxs-lookup"><span data-stu-id="fe9e0-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="fe9e0-103">Če uporabnik prejme opozorilo; **Nabiralnik arhiva je skoraj poln** ali pa morate povečati velikost nabiralnika arhiva, tukaj je nekaj namigov:</span><span class="sxs-lookup"><span data-stu-id="fe9e0-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="fe9e0-104">Če je uporabniku dodeljen paket Exchange Online, nadgradite na licenco **Exchange Online za paket 2** , da povečate velikost od 50 GB do 100GB.</span><span class="sxs-lookup"><span data-stu-id="fe9e0-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="fe9e0-105">Če je uporabnik že dodelil nekaj od tega: **Exchange Online (paket 2** ) ali Exchange Online (paket 1) z dodatkom za arhiviranje v storitvi Exchange Online, uporabite spodnje korake, da omogočite samodejno razširjanje arhiviranja:.</span><span class="sxs-lookup"><span data-stu-id="fe9e0-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="fe9e0-106">[Vzpostavite povezavo s storitvijo PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="fe9e0-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="fe9e0-107">Zaženite te unifiedgroup za uporabnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="fe9e0-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="fe9e0-108">Zaženite te unifiedgroup za potrditev, da je omogočena za uporabnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="fe9e0-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="fe9e0-109">Če želite več informacij, glejte:</span><span class="sxs-lookup"><span data-stu-id="fe9e0-109">For more information see:</span></span>

- [<span data-ttu-id="fe9e0-110"> Omogočanje neomejenega arhiviranja – pomoč za skrbnike – skladnost s predpisi Microsoft 365 | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="fe9e0-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="fe9e0-111">Omejitve za Exchange Online – opisi storitev | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="fe9e0-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="fe9e0-112">Nadgradnja na drug poslovni načrt | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="fe9e0-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

