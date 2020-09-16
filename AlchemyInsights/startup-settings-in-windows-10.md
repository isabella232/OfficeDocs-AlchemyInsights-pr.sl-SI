---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751151"
---
# <a name="startup-settings-in-windows-10"></a>Nastavitve zagona v sistemu Windows 10

**Spreminjanje, kateri programi se zaženejo samodejno ob zagonu**

1. Pojdite v razdelek [nastavitve > aplikacije > zagon](ms-settings:startupapps?activationSource=GetHelp).

2. Preverite, ali je vklopljen kateri koli program, ki ga želite zagnati ob **zagonu.**

**Dodajanje programa za samodejno izvajanje ob zagonu**

1. Kliknite ali tapnite **Start** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.

2. Z desno tipko miške kliknite program, kliknite **več**in nato kliknite **Odpri mesto datoteke**. Odpre se mesto, kjer je shranjena Bližnjica do programa. Če ni možnosti za odpiranje mesta datoteke, to pomeni, da se aplikacija ne more zagnati ob zagonu.

3. Ko je mesto datoteke odprto, pritisnite **tipko z logotipom sistema Windows + R**, vnesite **Shell: zagon**in nato kliknite **v redu**. Odpre se zagonska mapa.

4. Kopirajte in prilepite bližnjico do programa iz mesta datoteke v zagonsko mapo.

**Napredne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagon iz druge naprave)**

1. Shranite delo in zaprite vse odprte dokumente, ker bodo ti koraki znova zagnali računalnik.

2. Pojdite na [nastavitve > posodobitev & varnost > obnovitvijo](ms-settings:recovery?activationSource=GetHelp).

3. V razdelku **napredni zagon**kliknite **znova Zaženi zdaj**. 

4. Ko se računalnik znova zažene na zaslonu izberite možnost:

    - Če želite zagnati iz naprave, kot je pogon USB, kliknite **uporabi napravo**.

    - Če želite vnesti nastavitve UEFI (včasih se imenuje nastavitev BIOS-a), kliknite **Odpravljanje težav > napredne možnosti > nastavitve vdelane programske opreme UEFI**. 

    - Če želite vnesti varni način ali spremeniti napredne nastavitve zagona, kliknite **Odpravljanje težav > dodatnih možnosti > nastavitve zagona**in nato **znova Zaženi**. Morda boste pozvani k vnosu [obnovitvenega ključa za BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.