---
title: Samodejno premikanje e-poštnih sporočil v nabiralnik arhiva
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527099"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Samodejno premikanje e-poštnih sporočil v nabiralnik arhiva

Navodila za nastavitev pravilnika za samodejno premikanje stare e-pošte uporabnikov v arhivski nabiralnik:

1. Če želite [](https://go.microsoft.com/fwlink/p/?linkid=2077143)preveriti, ali je  >    >  bil za uporabnika omogočen arhivski nabiralnik, se po&te v **arhivu** za upravljanje podatkov o skladnosti. Če ni, kliknite **Omogoči** nato **da** v polju z opozorilom.
2. Pojdite v [**skrbniško središče za Exchange > upravljanje ustreznosti > oznak za hranjenje**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Izberite ikono +, nato pa izberite **samodejno uporabi za celoten nabiralnik**.
4. Dodelite ime oznaki za hranjenje in izberite **Premakni v Arhiv**. Za obdobje hranjenja vnesite želeni čas, na primer 90 dni. Kliknite **Shrani**.
5. Zdaj ustvarite pravilnik o hranjenju: izberite **Pravilniki o hranjenju**, izberite ikono za dodajanje novega pravilnika.
6. Dodelite ime pravilniku o hranjenju, nato pa kliknite in se pomaknite, da poiščete in dodate oznako hranjenja, ki ste jo pravkar ustvarili. Kliknite **Shrani**.
7. Na koncu uporabite pravilnik o hranjenju v nabiralniku uporabnika: še vedno v skrbniškem središču za Exchange odprite   >  **nabiralnike** prejemnikov. Izberite vse uporabnike, za katere želite uporabiti pravilnik, nato pa izberite **Uredi** (ikona svinčnika).
8. V pogovornem oknu kliknite **funkcije nabiralnika**. V razdelku **pravilnik o hranjenju** uporabite pravilnik, ki ste ga pravkar ustvarili > **Shrani**.
9. Če želite navodila za uporabo pravilnika za vse uporabnike, glejte [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
