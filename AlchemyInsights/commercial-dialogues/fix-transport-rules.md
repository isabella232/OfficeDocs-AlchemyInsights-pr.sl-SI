---
title: Popravljanje pravil prenosa
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750574"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="e27aa-102">Popravljanje pravil prenosa</span><span class="sxs-lookup"><span data-stu-id="e27aa-102">Fix transport rules</span></span>

<span data-ttu-id="e27aa-103">To sporočilo je vplivalo na pravilo za tok pošte po meri.</span><span class="sxs-lookup"><span data-stu-id="e27aa-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="e27aa-104">Če želite pregledati točno pravilo, naredite to:</span><span class="sxs-lookup"><span data-stu-id="e27aa-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="e27aa-105">V razdelku Rezultati pošiljanja v razdelku **dodatne informacije** si zapomnite **GUID** ali **ime pravilnika**.</span><span class="sxs-lookup"><span data-stu-id="e27aa-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="e27aa-106">Zaženite ukazno lupino za upravljanje Exchangea.</span><span class="sxs-lookup"><span data-stu-id="e27aa-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="e27aa-107">Če želite več informacij, glejte [odpiranje lupine za upravljanje Exchangea](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="e27aa-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="e27aa-108">Zaženite ta ukaz (z GUID-om iz vaše oddaje):  **TransportRule-Identity "GUID" | FL \* opis**\*</span><span class="sxs-lookup"><span data-stu-id="e27aa-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="e27aa-109">Če si želite ogledati konfigurirane pogoje, ki so vplivali na sporočilo, preglejte opis.</span><span class="sxs-lookup"><span data-stu-id="e27aa-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="e27aa-110">Če želite izvedeti več, glejte [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="e27aa-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>