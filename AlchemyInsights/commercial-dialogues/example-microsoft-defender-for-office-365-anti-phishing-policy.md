---
title: Primer programa Microsoft Defender za Office 365 za preprečevanje lažnega predstavljanja
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
- "9000760"
- "7391"
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035022"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primer programa Microsoft Defender za Office 365 za preprečevanje lažnega predstavljanja

Te nastavitve omogočajo pravilnik, imenovan *Domena in CEO*. Ta pravilnik zagotavlja zaščito uporabnika in domene pred poosebljavo in nato uporabi pravilnik za vsa e-poštna sporočila, ki jih prejmejo uporabniki v domeni. Najprej dodajte te informacije, da ustvarite pravilnik:

- **Ime**: Opis domene in **direktorja**: zagotavlja, da se ne poosebljata ceo in vaša domena.
  **Uporabljeno za**: Izberite **Domena prejemnika je**. V **razdelku Katero koli od** teh možnosti **izberite**, nato pa izberite domeno. Izberite **+ Dodaj**. Potrdite potrditveno polje ob imenu domene na seznamu (npr. contoso.com *),* nato pa izberite **Dodaj**. Izberite **Končano**.
- Ko ustvarite pravilnik, lahko natančno nastavite pravilnik tako, da uporabite te možnosti:
  - **Dodajanje uporabnikov za zaščito:** V tem primeru dodajte vsaj e-poštni naslov direktorja.
  - **Dodajte domene, ki jih želite** zaščititi: dodajte domeno organizacije, ki vključuje pisarno direktorja.
  - **Izberite dejanja:** **Za** Če je e-pošto poslal poosebljena oseba, izberite Preusmeri sporočilo na drug e-poštni naslov **in** nato vnesite e-poštni naslov varnostnega skrbnika (na primer *securityadmin@contoso.com*). Za **Če je e-pošto poslala poosebljena domena**, izberite **Pošlji v karanteno sporočilo**.
  - **Obveščanje o** nabiralniku: ta možnost je privzeto izbrana, ko ustvarite nov pravilnik za preprečevanje lažnega predstavljanja. Če želite najboljše **rezultate, pustite** to nastavitev »On«.
  - **Dodajte zaupanja vredne pošiljatelje in domene:** V tem primeru ne določite nobene preglasitve.
- Ko pregledate nastavitve, izberite Ustvari **ta pravilnik ali** **Shrani**, kot je primerno.

Če želite izvedeti več, glejte [Pravilniki za preprečevanje lažnega predstavljanja v Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
