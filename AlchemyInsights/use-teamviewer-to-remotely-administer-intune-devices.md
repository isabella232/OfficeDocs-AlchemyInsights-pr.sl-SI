---
title: Uporaba skupine TeamViewer za oddaljeno skrbništvo naprav Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555750"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Uporaba skupine TeamViewer za oddaljeno skrbništvo naprav Intune

Naprave, ki jih upravlja Intune, se lahko upravljajo na daljavo z [uporabo TeamViewer](https://www.teamviewer.com/).

Če želite upravljati Intune s funkcijo TeamViewer, uporabite te korake: 

Začnite s pridobivanjem poverilnic iz TeamViewer za nastavitev TeamViewer Connector na Intune. To omogoča admin, da vnesete poverilnice v TeamViewer Connector UI pod Naprave, enkratna operacija za vzpostavitev povezave med Intune in TeamViewer storitev.

**1. del: začetek seje z oddaljeno napravo**

1. V **razdelku Vse**naprave izberite napravo, s katerim želite začeti oddaljeno sejo.
2. Iz **... Več**, izberite **Nova seja oddaljene pomoči**.
3. Izberite **Da,** če želite potrditi, da želite vzpostaviti oddaljeno sejo.
    Ko storitev TeamViewer priznava zahtevo »Začetek nove oddaljene seje«, boste videli možnost **zagona oddaljene pomoči** pod podrobnostmi podokna »Pregled«ali »Essentials«) za napravo. Izberite **Kliknite več,** če želite razširiti podokno in prikazati stanje oddaljene pomoči.
4. Izberite **Zaženi oddaljeno** sejo, da sprožite sejo na skrbniški strani.
5. Izberite, ali želite prenesti binarno datoteko TeamViewer (Windows), in izberite **Zaženi**.<br/>
    ** Opomba** Prezrete lahko katero koli stran spletnega brskalnika, ki je odprta na spletnem mestu TeamViewer.

6. Potrdite zahtevo, da program TeamViewer spremeni napravo (samo windows).
7. Program TeamViewer se zažene in vključuje kodo seje za preverjanje pristnosti povezave z oddaljeno napravo.

**Del 2: Na napravi, ki je usmerjena v oddaljeno sejo**

1. Odprite portal podjetja Intune.
2. Poiščite zastavico obvestila: »Skrbnik za IT zahteva nadzor nad to napravo za sejo oddaljene pomoči« in izberite obvestilo.
3. Izberite prenos aplikacije TeamViewer ali potrdite prenos aplikacije TeamViewer iz trgovine z aplikacijami in izberite **Zaženi**.
    ** Opomba** Prezrete lahko katero koli stran spletnega brskalnika, ki je odprta na spletnem mestu TeamViewer.

4. Potrdite zahtevo, da program TeamViewer spremeni napravo (samo windows).
5. Program TeamViewer se zažene in vključuje kodo seje za preverjanje pristnosti povezave z oddaljeno napravo.
6. Pojavno okno vas vpraša, ali želite dovoliti začetek seje.

** Opomba** Kode sej, ki jih ustvari storitev TeamViewer, so samo enkratne uporabe. Če izgubite povezavo, morate:

1. Zaprite primerek aplikacije TeamViewer v oddaljeni napravi in skrbniški delovni postaji.
2. Zaprite portal podjetja v oddaljeni napravi.
3. Začnite novo »novo sejo oddaljene pomoči« iz skrbniškega portala.
4. Skozi okno portal podjetja v oddaljeni napravi uprite, da prejmete novo obvestilo.
5. Prenesite in odprite aplikacijo TeamViewer v oddaljeni napravi in skrbniški delovni postaji, kot prej.