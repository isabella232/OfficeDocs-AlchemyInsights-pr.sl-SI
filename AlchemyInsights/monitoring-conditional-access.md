---
title: Nadzorovanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708690"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nadzorovanje pogojnega dostopa za Exchange

Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije. Če želite razrešiti, priporočamo eno ali več od teh rešitev:

- Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja. Če ne, mora uporabnik vpisati napravo.
- V portalu Azure obiščite spletno mesto InTune > skladnost z napravo. V razdelku monitor kliknite skladnost naprave. Če želite preveriti, ali je naprava uporabnika označena kot združljiva, si oglejte poročilo o skladnosti naprave.
- V portalu Azure obiščite spletno mesto InTune > skladnost z napravo. V razdelku upravljanje kliknite pravilniki. Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika. Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave.
- Uredite uporabnikovo pogojno dostopno dodelitev.

1. V portalu Azure se pozanimajte za **Nastavitev**  >  pravilnikov **pogojnega dostopa**  >  .
2. Na seznamu izberite pravilnik.
3. Kliknite Uporabniki in skupine.
4. Če želite določene pravilnike usmeriti na osebo, jih dodajte na seznam vključi. Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na seznam izključi.

Uporabne povezave:

[Pregled skladnosti naprave](https://docs.microsoft.com/intune/device-compliance-get-started)

[Odpravljanje težav CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik za odpravljanje težav](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Nadzorovanje skladnosti naprave](https://docs.microsoft.com/intune/compliance-policy-monitor)

Opomba: ta navodila so koristna le za odpravljanje težav s pogojnim dostopom v storitvi Azure Active Directory. Možno je tudi, da karantena naprave blokira dostop do e-pošte s pravilnikom za Exchange. Več informacij o upravljanju Exchangeeve naprave lahko najdete [tukaj] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
