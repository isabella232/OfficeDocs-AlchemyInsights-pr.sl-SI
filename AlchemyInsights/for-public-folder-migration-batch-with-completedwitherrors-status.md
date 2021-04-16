---
title: Za selitveni paket javne mape s stanjem CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812480"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za selitveni paket javne mape s stanjem CompletedWithErrors

Če želite dokončati paket in iz preskočiti velike/slabe elemente, sledite tem korakom: 
1. Odobritev preskočenih elementov v selitvenih paketih:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Uporabite ta ukaz, če želite odobriti preskočene elemente v zahtevah za selitev, ki so »Sinhronizirane«, vendar niso dokončane:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Selitveni paket in zahteve bi se morali v nekaj minutah nadaljevati in dokončati.

