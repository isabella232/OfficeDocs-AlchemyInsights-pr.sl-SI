---
title: Ali morate označiti domeno ali pošiljatelja e-pošte varno?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319964"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Ali morate označiti domeno ali pošiljatelja e-pošte varno?

- Uporaba seznamov **varnih pošiljateljev ni** priporočljiva, saj v vaši organizaciji odpre napad za neželeno pošto, lažno predstavljanje in lažno predstavljanje.
- Če pa obstajajo poslovne zahteve, priporočamo, da **za** to uporabite pravila **[Flow pošto.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Z našimi navodili je mogoče zagotoviti preverjanje pristnosti pošiljatelja (preverjanje, da ni ponarejena domena). 
    **Opomba:** Priporočamo, da ne upravljate napačne pozitivne pošte z uporabo seznamov varnih pošiljateljev, saj lahko izjeme pri filtriranju neželene pošte odprejo organizacijo do varnostnih napadov. Če vaši uporabniki prejmejo sporočila, ki so nepravilno označena kot neželena ali neželena e-pošta, **[Prijavite sporočila in datoteke Microsoftu.](https://protection.office.com/reportsubmission)**
- Sef Pošiljateljem v storitvi Outlook, seznamu dovoljenih pošiljateljev ali seznamu  dovoljenih domen v pravilnikih za preprečevanje neželene pošte se je treba izogniti, saj pošiljatelji zaobidejo vso neželeno pošto, zaščito pred lažjo pošto in preverjanje pristnosti pošiljatelja (SPF, DKIM, DMARC). Ta način je najboljši za začasno preskušanje.
- Preverjanje, da je določena e-pošta obšla Vrednotenje neželene pošte, lahko preverite tako, da preverite glavo sporočila »X-Forefront-Antispam-Report« (SFV:SFE, SFV:SKA, SFV:SKN), glejte Glave sporočil za preprečevanje neželene **[pošte.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Ker želi Microsoft zagotoviti varnost svojih strank privzeto, [nekatere](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)preglasitve najemnika niso uporabljene za zlonamerno programsko opremo in lažno predstavljanje z visoko stopnjo zanesljivosti. Te preglasitve vključujejo: o Seznami dovoljenih pošiljateljev ali seznami dovoljenih domen (pravilniki za preprečevanje neželene pošte) o Outlook Sef pošiljateljev s seznamom dovoljenih naslovov IP (filtriranje povezave) 
- Edina preglasitev, ki omogoča, da sporočilo z lažnim predstavljanjem z visoko stopnjo zanesljivosti obide filtriranje Exchange pravila toka pošte (znana tudi kot pravila za prenos). Če želite za zaobiti filtriranje s pravili toka pošte, glejte Uporaba pravil toka pošte za nastavitev ravni zaupanja neželene pošte **[v sporočilih.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**