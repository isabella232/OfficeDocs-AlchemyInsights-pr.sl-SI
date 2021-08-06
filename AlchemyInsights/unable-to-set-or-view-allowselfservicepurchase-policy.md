---
title: Ni mogoče nastaviti ali si ogledati pravilnika AllowServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020208"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Ni mogoče nastaviti ali si ogledati pravilnika AllowServicePurchase

Pri poskusu nastaviti ali si ogledati pravilnik o nakupu AllowServicePurchase se prikaže to sporočilo o napaki:

*HandleError : Pravilnika o izdelku ni bilo mogoče pridobiti s Pravilnikid 'Allow NarHriServicePurchase', ErrorMessage – temeljna povezava je bila zaprta: Pri pošiljanju je prišlo do nepričakovane napake.*

Do tega lahko pride zaradi starejše različice programa Transport Layer Security (TLS). Če želite povezati storitev MSCommerce, morate uporabiti TLS 1.2 ali več.  

Če želite omogočiti/nastaviti protokol TLS na 1.2, ga preveriti in znova izvesti, poskusite to:
 1. V ukazni poziv lupine PowerShell (PS C: vnesite ta ukaz, če želite \) nastaviti protokol TLS na različico 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Preverite protokole TLS v uporabi s tem ukazom:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Po potrebi poskusite znova izvesti ukaze »Dobi« ali »Posodobi«.

