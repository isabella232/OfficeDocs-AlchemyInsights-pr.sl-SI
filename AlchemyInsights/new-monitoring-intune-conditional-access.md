---
title: Nadzor pogojnega dostopa do storitve Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327573"
---
# <a name="monitor-intune-conditional-access"></a>Nadzor pogojnega dostopa do storitve Intune

Uporabniki s pogojnim dostopom prejmejo e-poštno obvestilo, če ne izpolnjujejo zahtev za dostop, ki veljajo v vaši organizaciji. Če želite odpraviti to težavo, priporočamo, da odpravite eno ali več teh rešitev:

1. Če je videti, da je naprava vpisana, svetujte uporabniku, naj odpre aplikacijo Company Portal in preveri, ali je prikazana v Company Portal. Če naprava ni včlanjena, mora uporabnik napravo včlanjeti.
1. V portalu Azure pojdite v storitev **Intune**  >  **– skladnost naprave s predpisi.** 
1. Če si želite ogledati poročilo o skladnosti naprave s predpisi in preveriti, ali je uporabnikova naprava označena kot skladna s predpisi, v razdelku **Nadzor** kliknite **Skladnost naprave s predpisi.**
1. V portalu Azure pojdite v storitev **Intune**  >  **– skladnost naprave s predpisi.** V **razdelku Upravljanje** kliknite **Pravilniki.** Na seznamu pravilnikov za skladnost s predpisi preverite, ali je uporabnikovi napravi dodeljen profil. Če profil ni dodeljen, Intune ne more potrditi stanja skladnosti naprave s predpisi.
1. Uredite dodelitev uporabnikovega pogojnega dostopa.
1. V portalu Azure se pomaknite do možnosti Pravilniki o pogojnem dostopu do storitve **Intune**, na seznamu izberite pravilnik in kliknite Uporabniki in  >    >   **skupine.**
1. Če želite nekomu dodati določen pravilnik, ga dodajte na **seznam Vključi.** Če želite zagotoviti, da osebe ne bo več v pravilniku, jo dodajte na seznam **Izključi.**

**Koristne povezave:**

- [Pregled skladnosti naprave s predpisi](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Odpravljanje težav s ca-jem](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Pravilnik za odpravljanje težav](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Nadzorovanje skladnosti naprave s predpisi storitve Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Opomba:** Ta navodila so uporabna le pri odpravljanju težav s Azure Active Directory pogojnega dostopa. Napravo, ki blokira e-poštni dostop, lahko tudi karanteno s pravilnikom Exchange karanteno. Več informacij o upravljanju Exchange najdete [**tukaj.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
