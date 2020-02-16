---
title: Obnovitev izbrisane javne mape
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063748"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovitev izbrisane javne mape

**Če želite obnoviti izbrisane elemente iz javne mape**:

- [V outlooku 2016 ne morete obnoviti izbrisanih elementov iz javne mape, ki ni pošta](https://aka.ms/pfrec).
 
**Če želite obnoviti izbrisano javno mapo (katere koli vrste)**: 

- Prosimo, uporabite naslednje EXO PowerShell ukaz:

    Sintaksa:

    >$pf = dobi-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Ime-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. identiteta-pot \<pot, kjer bo mapa obnovljena>

    Primer: naslednji ukaz bo obnoviti Subfolder1 in ga postavite pod \Parent1:

    >$pf = dobi-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Ime-EQ "Subfolder1"}; Set-PublicFolder $pf. identiteta-pot \Parent1

Za več podrobnosti glejte [obnovitev izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
