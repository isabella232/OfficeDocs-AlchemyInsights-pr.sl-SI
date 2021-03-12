---
title: Primer Microsoftovega pravilnika za preprečevanje lažnega predstavljanja za Microsoft Defender za Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750797"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primer Microsoftovega pravilnika za preprečevanje lažnega predstavljanja za Microsoft Defender za Office 365

Te nastavitve omogočajo pravilnik, imenovan *domena in izvršni direktor*. Ta pravilnik zagotavlja zaščito uporabnika in domene pred poosebljanje, nato pa uporabi pravilnik za vse e-poštne pošte, ki jih prejmejo uporabniki v domeni. Najprej dodajte te informacije, da ustvarite pravilnik:

- **Ime**: domena in **Opis** CEO: zagotovite, da se direktor in vaša domena ne posnemata.
  **Uporabljeno za**: izberite **domeno prejemnika**. V razdelku **katero koli od teh** izberite **Izberi** in nato izberite domeno. Izberite **+ Dodaj**. Potrdite potrditveno polje ob imenu domene na seznamu (na primer *contoso.com*), nato pa izberite **Dodaj**. Izberite **Dokončano**.
- Ko je pravilnik ustvarjen, lahko prilagodite pravilnik tako, da uporabite te možnosti:
  - **Dodajanje uporabnikov za zaščito:** Za ta primer dodajte e-poštni naslov CEO na minimum.
  - **Dodajte domene za zaščito**: dodajte organizacijsko domeno, ki vključuje Office izvršnega direktorja.
  - **Izberite dejanja**: za **e-pošto, ki jo je poslal** lažni uporabnik, izberite **preusmeritev sporočila na drug e-poštni naslov**, nato pa vnesite e-poštni naslov varnostnega skrbnika (na primer *securityadmin@contoso.com*). **Če je e-pošta poslana z** lažno domeno, izberite **karantena sporočila**.
  - **Inteligenca nabiralnika**: Ta možnost je privzeto izbrana, ko ustvarite nov pravilnik za preprečevanje lažnega predstavljanja. To **Nastavitev pustite za najboljše** rezultate.
  - **Dodajanje zaupanja vrednih pošiljateljev in domen:** V tem primeru ne definirajte nobenega preglasitve.
- Ko pregledate nastavitve, izberite **Ustvari to pravilnik** ali **Shrani**, kot je primerno.

Če želite izvedeti več, glejte [Pravilniki za preprečevanje lažnega predstavljanja v programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
