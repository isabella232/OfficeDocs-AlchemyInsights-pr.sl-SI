---
title: Popravljanje uporabniških pravilnikov/nastavitev nabiralnika
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695901"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="6623e-102">Popravljanje uporabniških pravilnikov/nastavitev nabiralnika</span><span class="sxs-lookup"><span data-stu-id="6623e-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="6623e-103">Nastavitve neželene pošte v nabiralniku so vplivale na to sporočilo.</span><span class="sxs-lookup"><span data-stu-id="6623e-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="6623e-104">Če želite pregledati nastavitve, naredite to:</span><span class="sxs-lookup"><span data-stu-id="6623e-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="6623e-105">Zaženite ukazno lupino za upravljanje Exchangea.</span><span class="sxs-lookup"><span data-stu-id="6623e-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="6623e-106">Če želite več informacij, glejte [odpiranje lupine za upravljanje Exchangea](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="6623e-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="6623e-107">Zaženite ta ukaz (z uporabo e-poštnega naslova uporabnika):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="6623e-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="6623e-108">Preverite, ali je pošiljateljev e-poštni naslov del **TrustedSendersAndDomains** ali **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="6623e-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="6623e-109">Če je e-poštni naslov na enem od seznamov, ga boste morda morali odstraniti.</span><span class="sxs-lookup"><span data-stu-id="6623e-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="6623e-110">Če želite izvedeti več, glejte [set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="6623e-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
