---
title: Stanje senzorja za preverjanje končne točke programa Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676336"
---
# <a name="defender-endpoint-check-sensor-status"></a>Stanje senzorja za preverjanje končne točke programa Defender

Ploščica **Naprave s težavami s senzorjem** je na nadzorni plošči Varnostne operacije. Na tej ploščici so informacije o tem, kako posamezna naprava zagotavlja podatke senzorja in komunicira s storitvijo Defender for Endpoint Service. Poročilo poroča, koliko naprav zahteva pozornost in vam pomaga prepoznati naprave s težavo ter odpraviti znane težave.

Dva indikatorja stanja na ploščici ponujata informacije o številu naprav, ki storitvi ne poročajo pravilno:

- **Napačno konfigurirano** Naprave, ki morda delno poročajo podatke senzorja storitvi Defender for Endpoint service in lahko imajo napake pri konfiguraciji, ki jih je treba popraviti.
- **Nedejaven** Naprave, ki so prenehale poročanje storitvi Defender for Endpoint Service več kot sedem dni v preteklem mesecu.

Če kliknete katero koli od skupin, vas program usmeri na seznam Naprave, filtriran glede na vaše izbire. Na seznamu Naprave lahko filtrirate seznam stanj po tem stanju:

- **Aktivno** Naprave, ki se aktivno poročajo storitvi Defender for Endpoint Service.
- **Napačno konfigurirano** Naprave, ki morda delno poročajo podatke senzorja storitvi Defender for Endpoint service, vendar imajo napake pri konfiguraciji, ki jih je treba popraviti. Napačno konfigurirane naprave lahko imajo eno ali kombinacijo teh težav:

    - Brez podatkov senzorja – naprave so prenehale pošiljati podatke senzorja. Iz naprave se lahko sprožijo omejena opozorila.
    - Motnje komunikacije – zmožnost komunikacije z napravo je naglušna. Pošiljanje datotek v globinsko analizo, blokiranje datotek, izoliranje naprave iz omrežja in druga dejanja, pri katerih je potrebna komunikacija z napravo, morda ne bodo delovala.
- **Nedejaven** Naprave, ki so prenehale poročanje storitvi Defender for Endpoint Service.

S funkcijo za izvoz lahko prenesete celoten seznam v obliki zapisa CSV.

Če želite več informacij, glejte [Preverjanje stanja senzorjev v aplikaciji Microsoft Defender za končno točko.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Če želite več informacij o tem, kaj je povzročilo nedejavnost ali napačno konfigurirano napravo, glejte Popravljanje neprimernih senzorjev v [aplikaciji Microsoft Defender za končno točko](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
