---
title: Obnovitev izbrisane javne mape
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774547"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovitev izbrisane javne mape

**Če želite obnoviti izbrisane elemente iz javne mape**:

- Glejte [ne morete obnoviti izbrisanih elementov iz javne mape, ki ni pošta, v programu Outlook 2016](https://aka.ms/pfrec).
 
**Če želite obnoviti izbrisano javno mapo (katere koli vrste)**: 

- Uporabite naslednji ukaz EKSO PowerShell:

    Sintaksa

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: ta ukaz bo obnovil Subfolder1 in ga položil v \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Če želite več informacij, glejte [obnovitev izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
