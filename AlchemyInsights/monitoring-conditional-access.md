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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975117"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nadzorovanje pogojnega dostopa za Exchange

Uporabniki s pogojnim dostopom prejmejo e-poštno obvestilo, če ne izpolnjujejo zahtev za dostop, ki veljajo v vaši organizaciji. Če želite odpraviti to težavo, priporočamo, da odpravite eno ali več teh rešitev:

- Če je videti, da je naprava včlaljena, svetujte uporabniku, naj odpre aplikacijo Company Portal in preveri, ali je prikazana v Company Portal. Če naprava ni včlanjena, mora uporabnik napravo včlanite.
- V portalu Azure pojdite Intune ali > naprave. V razdelku Nadzor kliknite Skladnost naprave s predpisi. Oglejte si poročilo o skladnosti naprave s predpisi, da preverite, ali je uporabnikova naprava označena kot skladna s predpisi.
- V portalu Azure pojdite Intune ali > naprave. V razdelku Upravljanje kliknite Pravilniki. Na seznamu pravilnikov za skladnost s predpisi preverite, ali je uporabnikovi napravi dodeljen profil. Če profil ni dodeljen, Intune ne more potrditi stanja skladnosti naprave s predpisi.
- Uredite dodelitev uporabnikovega pogojnega dostopa.

1. V portalu Azure pojdite na **Pravilniki o pogojnem dostopu do storitve Intune.**  >    >  
2. Na seznamu izberite pravilnik.
3. Kliknite Uporabniki in skupine.
4. Če želite določeni ravni ciljati določen pravilnik določene osebe, jo dodajte na seznam Vključi. Če želite zagotoviti, da osebe ne bo več v pravilniku, jo dodajte na seznam Izključi.

Koristne povezave:

[Pregled skladnosti naprave s predpisi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Odpravljanje težav s ca-jem](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik za odpravljanje težav](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Nadzorovanje skladnosti naprave s predpisi storitve Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Opomba: ta navodila so uporabna le pri odpravljanju težav s Azure Active Directory pogojnega dostopa. Napravo, ki blokira e-poštni dostop, lahko tudi karanteno s pravilnikom Exchange pošte. Več informacij o Exchange napravah najdete [tukaj]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
