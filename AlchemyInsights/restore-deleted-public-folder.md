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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158540"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovitev izbrisane javne mape

**Če želite obnoviti izbrisane elemente iz javne mape**:

- [V outlooku 2016 ne morete obnoviti izbrisanih elementov iz javne mape, ki ni pošta](https://aka.ms/pfrec).
 
**Če želite obnoviti izbrisano javno mapo (katere koli vrste)**: 

- Prosimo, uporabite naslednje EXO PowerShell ukaz:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: naslednji ukaz bo obnoviti Subfolder1 in ga postavite pod \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Za več podrobnosti glejte [obnovitev izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
