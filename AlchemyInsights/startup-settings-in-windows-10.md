---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409229"
---
# <a name="startup-settings-in-windows-10"></a>Nastavitve zagona v sistemu Windows 10

**Spreminjanje aplikacij, ki se samodejno zaženejo ob zagonu**

1. Odprite [nastavitve > aplikacije > zagon](ms-settings:startupapps?activationSource=GetHelp).

2. Preverite, ali je aplikacija, ki jo želite zagnati ob zagonu, **vklopljena.**

**Dodajanje aplikacije za samodejno izvajanje ob zagonu**

1. Kliknite ali tapnite **Začni** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.

2. Z desno miškino tipko kliknite aplikacijo, kliknite **več**in nato kliknite **Odpri mesto datoteke**. S tem se odpre mesto, kjer je shranjena Bližnjica do aplikacije. Če ni možnosti za odpiranje mesta datoteke, to pomeni, da se aplikacija ne more zagnati ob zagonu.

3. Ko je mesto datoteke odprto, pritisnite **tipko z logotipom Windows + R**, vnesite **Shell: zagon**in kliknite **v redu**. To odpre mapo Startup.

4. Kopirajte in prilepite bližnjico do aplikacije iz mesta datoteke v mapo Startup.

**Napredne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagonom iz druge naprave)**

1. Shranite svoje delo in zaprite vse odprte dokumente, saj bodo ti koraki znova zagnali računalnik.

2. Odprite [nastavitve > posodobitev & varnost > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Pod **naprednim zagonom**kliknite **znova Zaženi zdaj**. 

4. Po vnovičnem zagonu računalnika na izberite zaslon z možnostmi:

    - Če želite zagnati napravo, kot je pogon USB, kliknite **uporabi napravo**.

    - Če želite vnesti nastavitve UEFI (včasih imenovane nastavitve BIOS-a), kliknite **Odpravljanje težav > napredne možnosti > nastavitve vdelane programske opreme UEFI**. 

    - Če želite vnesti varni način ali spremeniti napredne nastavitve zagona, kliknite **Odpravljanje težav > napredne možnosti > nastavitve zagona**, nato kliknite **vnovični zagon**. Morda boste morali vnesti [obnovitveni ključ za BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.