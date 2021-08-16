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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025518"
---
# <a name="monitor-intune-conditional-access"></a>Nadzor pogojnega dostopa do storitve Intune

Uporabniki s pogojnim dostopom prejmejo e-poštno obvestilo, če ne izpolnjujejo zahtev za dostop, ki veljajo v vaši organizaciji. Če želite odpraviti to težavo, priporočamo, da odpravite eno ali več teh rešitev:

1. Če je videti, da je naprava včlaljena, svetujte uporabniku, naj odpre aplikacijo Company Portal in preveri, ali je prikazana v Company Portal. Če naprava ni včlanjena, mora uporabnik napravo včlanjeti.
1. V portalu Azure pojdite v storitev **Intune**  >  **– skladnost naprave s predpisi.** 
1. Če si želite ogledati poročilo o skladnosti naprave s predpisi in preveriti, ali je uporabnikova naprava označena kot skladna s predpisi, v razdelku **Nadzor** kliknite **Skladnost naprave s predpisi.**
1. V portalu Azure pojdite v storitev **Intune**  >  **– skladnost naprave s predpisi.** V **razdelku Upravljanje** kliknite **Pravilniki.** Na seznamu pravilnikov za skladnost s predpisi preverite, ali je uporabnikovi napravi dodeljen profil. Če profil ni dodeljen, Intune ne more potrditi stanja skladnosti naprave s predpisi.
1. Uredite dodelitev uporabnikovega pogojnega dostopa.
1. V portalu Azure se pomaknite do možnosti Pravilniki pogojnega dostopa do storitve **Intune**, na seznamu izberite pravilnik in kliknite Uporabniki in  >    >   **skupine.**
1. Če želite nekomu dodati določen pravilnik, ga dodajte na **seznam Vključi.** Če želite zagotoviti, da osebe ne bo več v pravilniku, jo dodajte na seznam **Izključi.**

**Koristne povezave:**

- [Pregled skladnosti naprave s predpisi](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Odpravljanje težav s ca-jem](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Pravilnik za odpravljanje težav](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Nadzorovanje skladnosti naprave s predpisi storitve Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ta navodila so uporabna le pri odpravljanju težav z Azure Active Directory funkcije pogojnega dostopa. Napravo, ki blokira e-poštni dostop, lahko tudi karanteno s pravilnikom Exchange pošte. Več informacij o upravljanju Exchange najdete [**tukaj.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
