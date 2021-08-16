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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068180"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za selitveni paket javne mape s stanjem CompletedWithErrors

Če želite dokončati paket in iz preskočiti velike/slabe elemente, sledite tem korakom: 
1. Odobritev preskočenih elementov v selitvenih paketih:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Uporabite ta ukaz, če želite odobriti preskočene elemente v zahtevah za selitev, ki so »Sinhronizirane«, vendar niso dokončane:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Selitveni paket in zahteve bi se morali v nekaj minutah nadaljevati in dokončati.

