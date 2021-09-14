---
title: Omejitev prejemanja nabiralnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316034"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Omejitev prejemanja nabiralnika

Microsoft je pred kratkim začel uveljavljati prag na nabiralnik, ki je 3600 sporočil na uro. Če želite več informacij, [Exchange Online omejitve.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 nabiralniki, ki prejmejo več kot 3600 sporočil v eni uri, so dušeni za naslednjih 60 min. 

Poleg tega je uporabljena omejitev parov pošiljatelj-prejemnik (SRP), ki blokira sporočila, ki jih je prejel Microsoft 365 nabiralnik uporabnika določenega pošiljatelja. Če en pošiljatelj pošlje več kot 33 % skupnega praga ali 1200 sporočil na z zaporedno uro za določenega prejemnika, se odpre omejitev za najbolj srp, nabiralnik pa ne sprejme več sporočil tega pošiljatelja. Upoštevajte to:

- Ta omejitev je aplikacija za e-pošto, prejeto iz drugih najemnikov, pošiljateljev na mestu uporabe ali internetnih pošiljateljev.
- Dostava e-pošte v nabiralnik je blokirana naslednjih 60 minut. 
- Pošiljatelji v te nabiralnike prejmejo poročilo o dostavi (5.2.121 ali 5.2.122), v katerem je navedeno, da je nabiralnik presegel največji prag dostave. Znotraj najemnika (pošta znotraj istega najemnika) je še vedno dostavljena.
- Ko je uporabljena omejitevRP, nabiralnik prejemnika še naprej sprejema sporočila drugih pošiljateljev.

Skrbniki lahko spremljajo trenutno dejavnost nabiralnika tako, da dostopajo do novega poročila in vpogleda v skrbniškem središču za Exchange, ki se imenuje »Nabiralniki, ki presegajo omejitve prejemanja«. Vpogled je prikazan le, če najemnik ni vnezla nabiralnikov, medtem ko je poročilo vedno prikazano na nadzorni plošči, vendar je prazno, razen če najemnik ni preglasil nabiralnikov.

Če želite več informacij o omejivah sprejemanja vpogledov, glejte Nabiralniki, ki presegajo vpogled v omejitve prejemanja [v novem EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Če želite več informacij o poročilu o preseganju omejitev sprejemanja, glejte Poročilo o nabiralnikih, ki presegajo omejitve sprejemanja [v novem EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)