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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792148"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Ali morate označiti domeno ali pošiljatelja e-pošte varno?

- Uporaba seznamov **varnih pošiljateljev ni** priporočljiva, saj v vaši organizaciji odpre napad za neželeno pošto, lažno predstavljanje in lažno predstavljanje.
- Če pa obstajajo poslovne zahteve, priporočamo, **da za** to uporabite **[pravila](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** toka pošte. Z našimi navodili je mogoče zagotoviti, da je preverjanje pristnosti pošiljatelja (preverjanje, da ni ponarejena domena). **Opomba:** Priporočamo, da ne upravljate napačne pozitivne pošte z uporabo seznamov varnih pošiljateljev, saj lahko izjeme pri filtriranju neželene pošte odprejo organizacijo do varnostnih napadov. Če vaši uporabniki prejmejo sporočila, ki so nepravilno označena kot neželena ali neželena e-pošta, prijavite **[sporočila in datoteke Microsoftu.](https://protection.office.com/reportsubmission)**
- Varnim pošiljateljem v Outlooku, seznamu dovoljenih pošiljateljev  ali seznamu dovoljenih domen v pravilnikih za preprečevanje neželene pošte se je treba izogniti, saj pošiljatelji zaobidejo vso neželeno pošto, zaščito pred lažjo zaščito in preverjanje pristnosti pošiljatelja (SPF, DKIM, DMARC). Ta način je najboljši za začasno preskušanje.
