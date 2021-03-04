---
title: Nadzorovanje pogojnega dostopa za InTune
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428307"
---
# <a name="monitor-intune-conditional-access"></a>Nadzorovanje pogojnega dostopa za InTune

Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije. Če želite razrešiti, priporočamo eno ali več od teh rešitev:

1. Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja. Če ne, mora uporabnik vpisati napravo.
1. V portalu **Azure se pozanimajte o**  >  **skladnosti naprave**. 
1. Če si želite ogledati poročilo o skladnosti naprave, da preverite, ali je naprava uporabnika označena kot združljiva, v razdelku **monitor** kliknite **skladnost naprave**.
1. V portalu **Azure se pozanimajte o**  >  **skladnosti naprave**. V razdelku **upravljanje** kliknite **Pravilniki**. Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika. Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave.
1. Uredite uporabnikovo pogojno dostopno dodelitev.
1. V portalu Azure se pomaknite do možnosti **Prilagodi**  >  pravilnike **pogojnega dostopa**  >  , na seznamu izberite pravilnik in kliknite **Uporabniki in skupine**.
1. Če želite določene pravilnike usmeriti na osebo, jih dodajte na **seznam vključi**. Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na **seznam izključi**.

**Uporabne povezave:**

- [Pregled skladnosti naprave](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Odpravljanje težav CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Pravilnik za odpravljanje težav](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Nadzorovanje skladnosti naprave](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ti koraki so v pomoč pri odpravljanju težav s pogojnim dostopom v storitvi Azure Active Directory. Možno je tudi, da karantena naprave blokira dostop do e-pošte s pravilnikom za Exchange. Več informacij o upravljanju naprav Exchange lahko najdete [**tukaj**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
