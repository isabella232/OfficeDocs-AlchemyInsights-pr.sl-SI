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
# <a name="hide-public-folders"></a>Skrivanje javnih map

**Če želite skriti celotno drevo javnih map**:

S koraki v [tem](https://aka.ms/ControlPF) članku lahko skrijete celotno drevo javnih map od selektivnih ali vseh uporabnikov.

**Če želite skriti določeno javno mapo**:

1. Dodajanje dovoljenj za uporabnike, ki potrebujejo dostop do javne mape

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Odstranjevanje **privzetega** uporabnika s seznama **dovoljenj** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
