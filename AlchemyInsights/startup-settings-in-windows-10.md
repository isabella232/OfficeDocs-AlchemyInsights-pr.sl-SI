---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828168"
---
# <a name="startup-settings-in-windows-10"></a>Nastavitve zagona v sistemu Windows 10

**Spreminjanje, katere aplikacije se samodejno zaženejo ob zagonu**

1. Odprite Nastavitve [in >, > zagonu.](ms-settings:startupapps?activationSource=GetHelp)

2. Prepričajte se, da je kateri koli program, ki ga želite zagnati ob zagonu, **vklopljen.**

**Dodajanje programa za samodejni zagon ob zagonu**

1. Kliknite ali tapnite **Začetni meni** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.

2. Z desno tipko miške kliknite program, **kliknite Več** in nato Odpri **mesto datoteke.** S tem odprete mesto, kjer je shranjena bližnjica do aplikacije. Če možnost Odpri mesto datoteke ni na voljo, to pomeni, da se program ne more zagnati ob zagonu.

3. Ko je mesto datoteke odprto, pritisnite tipko **z logotipom sistema Windows + R**, vnesite **shell:startup**, nato pa kliknite V **redu**. S tem odprete mapo Zagon.

4. Kopirajte in prilepite bližnjico do programa z mesta datoteke v zagonsko mapo.

**Dodatne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagonom iz druge naprave)**

1. Shranite svoje delo in zaprite vse odprte dokumente, saj boste s temi koraki znova zagnali računalnik.

2. Pojdite na [Nastavitve in > Posodobite & obnovitev > varnost.](ms-settings:recovery?activationSource=GetHelp)

3. V **razdelku Napredni zagon** kliknite Znova **zaženi** zdaj. 

4. Ko se računalnik znova zažene, se prikaže zaslon za izbiro možnosti:

    - Če se želite zagnati iz naprave, kot je pogon USB, **kliknite Uporabi napravo**.

    - Če želite vnesti nastavitve UEFI (imenujemo jih tudi namestitev SETUP) > Dodatne možnosti **> nastavitvah vdelane programske opreme UEFI**. 

    - Če želite vnesti varni način ali spremeniti dodatne nastavitve zagona, **> Dodatne možnosti > zagona**, nato pa kliknite Znova **zaženi.** Morda boste morali vnesti obnovitveni [ključ za BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.