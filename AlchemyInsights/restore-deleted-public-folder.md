---
title: Obnovitev izbrisane javne mape
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
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943391"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovitev izbrisane javne mape

**Obnovitev izbrisanih elementov iz javne mape:**

- Glejte [Izbrisanih elementov ni mogoče obnoviti iz javne mape, ki ni poštna, v Outlook 2016.](https://aka.ms/pfrec)
 
**Če želite obnoviti izbrisano javno mapo (katere koli vrste):** 

- Uporabite ta ukaz EXO PowerShell:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: The following command will restore Subfolder1 and place it under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Če [želite več podrobnosti, glejte Obnovitev izbrisane](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) javne mape.
