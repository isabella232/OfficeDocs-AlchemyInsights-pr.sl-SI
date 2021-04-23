---
title: Pravilniki o hranjenju v Skrbniškem središču za Exchange ne delujejo
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952244"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravilniki o hranjenju v Skrbniškem središču za Exchange

Če želite, da zaženemo avtomatizirana preverjanja za spodaj omenjene nastavitve, izberite gumb »Nazaj« < – na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s pravilniki o hranjenju.

Če imate težave s pravilniki o hranjenju v Skrbniškem središču za Exchange, ki se ne uporabljajo za nabiralnike ali elemente, ki se ne premaknejo v nabiralnik arhiva, preverite to:

**Korenski vzroki:**

- **Pomočnik za upravljane** mape ni obdelal uporabnikovega nabiralnika. Pomočnik za upravljane mape poskuša obdelati vsak nabiralnik v organizaciji v oblaku enkrat na sedem dni.

  **Rešitev:** Zaženite pomočnika za upravljane mape.

- **Zadržanje** hranjenja **je bilo omogočeno** za nabiralnik. Če je bil nabiralnik v zadržanju hranjenja, se v tem času pravilnik o hranjenju za nabiralnik ne bo obdelal.

  **Rešitev:** Preverite stanje nastavitve zadržanja in po potrebi posodobite. Če želite več informacij, glejte [Zadržanje hranjenja nabiralnika.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.
 
Če želite več informacij o pravilnikih o hranjenju v Skrbniškem središču za Exchange, glejte:

- [Oznake za hranjenje in pravilniki o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ali [dodajanje ali odstranjevanje oznak za hranjenje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako prepoznati vrsto zadržanja v nabiralniku](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
