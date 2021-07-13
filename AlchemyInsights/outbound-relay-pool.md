---
title: Outbound relay pool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381863"
---
# <a name="outbound-relay-pool"></a>Outbound relay pool

Microsoft bo konfiguracijo za posredovanje ali posredovanje e-pošte prek e-pošte Microsoft 365. Sporočila v določenih scenarijih so posredovana ali posredovana prek Microsoft 365 uporabo posebne skupine posredovanja. Sporočila, poslana s pomočjo skupine prejemnikov, so lahko v mapi z neželeno pošto prejemnika. Če želite več informacij, glejte [Skupine odhodnih dostav](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Če se želite izogniti scenariju z uporabo skupine posredovanje, se prepričajte, da posredovana/posredovana sporočila izpolnjujejo enega od teh pogojev:

- Odhodni pošiljatelj je sprejeta domena najemnika.
- Ogrodje SPF (Sender Policy Framework) se poda, ko je sporočilo Microsoft 365.
- DomainKeys Identified Mail (DKIM) v domeni pošiljatelja P2 poda sporočilo, ko se sporočilo Microsoft 365.
 
Sporočila, ki ustrezajo zgornjim pogojem, niso posredovala prek skupine posredovanje.

Če je zapis MX za vašo domeno usmerjen v strežnik tretje osebe ali strežnik na mestu uporabe, uporabite izboljšano filtriranje in se prepričajte, da je preverjanje veljavnosti SPF pravilno za dohodno e-pošto in da preprečite pošiljanje e-pošte prek skupine posredovanje.

**Kako lahko vemo, ali je to vplivalo na nas v poolu za posredovanje?**

Če posredovana ali posredovana e-poštna sporočila uporabljajo enega od zgornjih pogojev, sporočila ne bodo posredovana prek skupine posredovanje. Če pa je sporočilo poslano prek skupine posredovalnih strežnikov, je IP odhodnega strežnika v obsegu 40.95.0.0/16, ime odhodnega strežnika pa je v imenu vključuje **rly.**

