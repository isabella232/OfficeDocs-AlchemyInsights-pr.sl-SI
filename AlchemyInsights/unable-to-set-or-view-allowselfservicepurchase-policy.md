---
title: Pravilnika AllowSelfServicePurchase ni mogoče nastaviti ali si ogledati
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735215"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Pravilnika AllowSelfServicePurchase ni mogoče nastaviti ali si ogledati

Pri poskusu nastavljanja ali ogleda pravilnika AllowSelfServicePurchase se prikaže to sporočilo o napaki:

*HandleError: ni bilo mogoče pridobiti pravilnika o izdelku z PolicyId» AllowSelfServicePurchase «,» errorMessage «– osnovna povezava je bila zaprta: Nepričakovana napaka pri pošiljanju.*

To je morda zaradi starejše različice varnosti transportne plasti (TLS). Če želite vzpostaviti povezavo s storitvijo MSCommerce, morate uporabiti TLS 1,2 ali novejšo.  

Upoštevajte spodnja navodila za omogočanje/nastavitev protokola TLS v 1,2, preverjanje in vnovičen poskus.
 1. V ukazni vrstici lupine PowerShell (PS C: \) vnesite ta ukaz, da nastavite protokol TLS na različico 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Preverjanje protokola TLS v uporabi s tem ukazom:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Po potrebi znova poskusite izvesti ukaze Get ali Update.

