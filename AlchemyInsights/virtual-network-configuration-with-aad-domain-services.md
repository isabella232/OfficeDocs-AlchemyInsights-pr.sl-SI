---
title: Navidezna konfiguracija s storitvami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885650"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Navidezna konfiguracija s storitvami

Navidezna konfiguracija s storitvijo storitev za ZVOČNO premišljene domene vključuje te korake: 

1. Preverjanje zdravja domene na portalu Azure https://aka.ms/aadds-health
2. Preverjanje NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v domenskih storitvah storitve Azure AD v portalu https://aka.ms/aadds-networking
3. Zagotovite, da je navidezno omrežje razporejeno v isti regiji Azure kot domena storitve Azure AD Domain Services.
4. Zagotavljanje, da nimate obstoječe domene z istim imenom domene, ki je na voljo v navideznem omrežju.

Če želite več informacij o načrtovanju načrtovanja v navideznem omrežju Azure, da boste podpirali storitve storitev s pozdravnimi domenami, glejte [navidezna omrežna](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

