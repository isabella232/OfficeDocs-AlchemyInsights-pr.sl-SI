---
title: Skrivanje javnih map
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315440"
---
# <a name="hide-public-folders"></a><span data-ttu-id="f8034-102">Skrivanje javnih map</span><span class="sxs-lookup"><span data-stu-id="f8034-102">Hide public folders</span></span>

<span data-ttu-id="f8034-103">**Če želite skriti celotno drevo javnih map**:</span><span class="sxs-lookup"><span data-stu-id="f8034-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="f8034-104">S koraki v [tem](https://aka.ms/ControlPF) članku lahko skrijete celotno drevo javnih map od selektivnih ali vseh uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="f8034-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="f8034-105">**Če želite skriti določeno javno mapo**:</span><span class="sxs-lookup"><span data-stu-id="f8034-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="f8034-106">Dodajanje dovoljenj za uporabnike, ki potrebujejo dostop do javne mape</span><span class="sxs-lookup"><span data-stu-id="f8034-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="f8034-107">Odstranjevanje **privzetega** uporabnika s seznama **dovoljenj** :</span><span class="sxs-lookup"><span data-stu-id="f8034-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
