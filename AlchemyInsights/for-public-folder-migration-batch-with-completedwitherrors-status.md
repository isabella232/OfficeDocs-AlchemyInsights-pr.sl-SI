---
title: Za selitev javnih map s stanjem» CompletedWithErrors «
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043619"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za selitev javnih map s stanjem» CompletedWithErrors «

Uporabite naslednje korake za dokončanje serije, preskoči velike/slabe elemente: 
1. Odobrite izpuščene elemente v selitvenem paketu:

    Set-MigrationBatch \<batchname>-Odobriteskippeditems 
2. S tem ukazom odobrite izpuščene elemente v zahtevah za selitev, ki so» sinhronizirani «, vendar niso končani:

    $pf = zahteva za Get-PublicFolderMailboxMigrationRequest | Get-Publicfoldermailboxmigrationrequeststatistika-IncludeReport; ForEach ($i v $pf) {IF ($i. LargeItemsEncountered-gt 0-ali $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-Skippeditemodobritaltime $ ([DateTime]:: UtcNow)}}
3. Selitveni paket in zahteve se morajo nadaljevati in dokončati v nekaj minutah.

