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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059242"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Samodejno premikanje e-poštnih sporočil v nabiralnik arhiva

Pravilnik nastavite tako, da samodejno premakne uporabnikovo staro e-pošto v nabiralnik arhiva:

1. Če želite [**preveriti, ali je nabiralnik arhiva**](https://go.microsoft.com/fwlink/p/?linkid=2077143)omogočen za uporabnika, odprite arhiv za upravljanje varnosti in & za  >    >   skladnost s predpisi. Če ni, v polju z **opozorilom** **kliknite** Omogoči in nato Da.
2. Obiščite [**skrbniško Exchange in > za skladnost > oznake za hranjenje.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Izberite ikono + in nato izberite samodejno **uporabi za celoten nabiralnik.**
4. Oznaki za hranjenje dodelite ime in izberite **Premakni v arhiv.** Za obdobje hranjenja vnesite čas, ki ga želite, na primer 90 dni. Kliknite **Shrani**.
5. Zdaj ustvarite pravilnik o hranjenju: izberite **pravilniki o** hranjenju , izberite ikono, da dodate nov pravilnik.
6. Pravilniku o hranjenju dodelite ime, nato pa kliknite in se pomaknite, da najdete in dodate oznako za hranjenje, ki ste jo pravkar ustvarili. Kliknite **Shrani**.
7. Nato uporabite pravilnik o hranjenju za nabiralnik uporabnika: še vedno v skrbniškem središču za Exchange pojdite v   >  **nabiralnike prejemnikov.** Izberite vse uporabnike, za katerega želite uporabiti pravilnik, nato pa izberite **Uredi** (ikona svinčnika).
8. V pogovornem oknu kliknite Funkcije **nabiralnika.** V **razdelku Pravilnik o** hranjenju uporabite pravilnik, ki ste ga pravkar ustvarili > **Shrani.**
9. Če želite navodila za uporabo pravilnika za vse uporabnike, [glejte Uporaba pravilnika o hranjenju za nabiralnike.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
