---
title: Omogočanje vdelovanje podedovanih pogovornih okna za odpiranje poročil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003405"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogočanje vdelovanje podedovanih pogovornih okna za odpiranje poročil

**Težava**

Uporabniki ne morejo odpreti poročil. »Nekaj je šlo narobe. Za več informacij si preberite tehnične podrobnosti.«

**Vzrok**

Poročil ni mogoče naložiti v UCI z napako »Opis obrazca je »null« ali ni definiran.« Za poročila v uporabniškem vmesniku še vedno potrebujete podedovana pogovorna okna, zato mora imeti sistem stranke omogočeno možnost *allowlegacydialogsembedding.*

**Rešitev**

1. Pojdite na **zavihek Nastavitve >Skrbnik > System Nastavitve > Splošno.**

2. Nastavitev »Omogoči vdelovanje določenih podedovanih pogovornih okna v odjemalcu brskalnika poenotenega vmesnika« na **Da.**
