---
title: Obnovitev izbrisanih elementov z ukazom cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835827"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="6ede9-102">Obnovitev izbrisanih elementov z ukazom cmdlet</span><span class="sxs-lookup"><span data-stu-id="6ede9-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="6ede9-103">Uporabite ukaz [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet za ogled izbrisanih elementov v nabiralnikih.</span><span class="sxs-lookup"><span data-stu-id="6ede9-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="6ede9-104">Ko najdete izbrisane elemente, jih obnovite z ukazom [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="6ede9-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="6ede9-105">Vse podrobnosti najdete v [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6ede9-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="6ede9-106">Pred zagonom ukaza cmdlet morate imeti dodeljeno vlogo za uvoz in izvoz nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="6ede9-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="6ede9-107">Če želite več informacij, glejte [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="6ede9-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
