---
title: Pravilniki o hranjenju Exchange skrbniškem središču ne delujejo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074948"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravilniki o hranjenju Exchange skrbniškem središču

Če želite, da zaženemo avtomatizirana preverjanja za spodaj omenjene nastavitve, izberite gumb »Nazaj« < – na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s pravilniki o hranjenju.

Če imate težave s pravilniki o hranjenju v skrbniškem središču za Exchange ki se ne uporabljajo za nabiralnike ali elemente, ki se ne premikajo v nabiralnik arhiva, preverite to:

**Korenski vzroki:**

- **Pomočnik za upravljane** mape ni obdelal uporabnikovega nabiralnika. Pomočnik za upravljane mape poskuša obdelati vsak nabiralnik v organizaciji v oblaku enkrat na sedem dni.

  **Rešitev:** Zaženite pomočnika za upravljane mape.

- **Zadržanje** hranjenja **je bilo omogočeno** za nabiralnik. Če je bil nabiralnik v zadržanju hranjenja, se v tem času pravilnik o hranjenju za nabiralnik ne bo obdelal.

  **Rešitev:** Preverite stanje nastavitve zadržanja in po potrebi posodobite. Če želite več informacij, glejte [Zadržanje hranjenja nabiralnika.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.
 
Če želite več informacij o pravilnikih o hranjenju v Exchange skrbniškem središču, glejte:

- [Oznake za hranjenje in pravilniki o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ali [dodajanje ali odstranjevanje oznak za hranjenje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako prepoznati vrsto zadržanja v nabiralniku](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
