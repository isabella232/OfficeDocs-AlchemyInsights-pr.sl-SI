---
title: Paket selitve javne mape z CompletedWithErrors stanjem
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744129"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Paket selitve javne mape z CompletedWithErrors stanjem

S temi koraki lahko dokončate paket, preskočite velike/slabe elemente: 
1. Odobritev izpuščenih elementov v selitvenem paketu:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Uporabite ta ukaz, če želite odobriti izpuščene elemente za selitvene zahteve, ki so» sinhronizirane «, vendar niso dokončane:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Selitveni paket in zahteve naj se nadaljujejo in dokončajo v nekaj minutah.

