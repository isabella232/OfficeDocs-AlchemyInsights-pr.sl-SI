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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="b184d-102">Obnovitev izbrisane javne mape</span><span class="sxs-lookup"><span data-stu-id="b184d-102">Restore a deleted public folder</span></span>

<span data-ttu-id="b184d-103">**Če želite obnoviti izbrisane elemente iz javne mape**:</span><span class="sxs-lookup"><span data-stu-id="b184d-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="b184d-104">[V outlooku 2016 ne morete obnoviti izbrisanih elementov iz javne mape, ki ni pošta](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="b184d-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="b184d-105">**Če želite obnoviti izbrisano javno mapo (katere koli vrste)**:</span><span class="sxs-lookup"><span data-stu-id="b184d-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="b184d-106">Prosimo, uporabite naslednje EXO PowerShell ukaz:</span><span class="sxs-lookup"><span data-stu-id="b184d-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="b184d-107">Sintaksa:</span><span class="sxs-lookup"><span data-stu-id="b184d-107">Syntax:</span></span>

    ><span data-ttu-id="b184d-108">$pf = dobi-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Ime-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. identiteta-pot \<pot, kjer bo mapa obnovljena></span><span class="sxs-lookup"><span data-stu-id="b184d-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="b184d-109">Primer: naslednji ukaz bo obnoviti Subfolder1 in ga postavite pod \Parent1:</span><span class="sxs-lookup"><span data-stu-id="b184d-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="b184d-110">$pf = dobi-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Ime-EQ "Subfolder1"}; Set-PublicFolder $pf. identiteta-pot \Parent1</span><span class="sxs-lookup"><span data-stu-id="b184d-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="b184d-111">Za več podrobnosti glejte [obnovitev izbrisane javne mape](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="b184d-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
