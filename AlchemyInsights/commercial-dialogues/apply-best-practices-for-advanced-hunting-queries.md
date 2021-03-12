---
title: Uporaba najboljših praks za napredne poizvedbe za lov
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749549"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Uporaba najboljših praks za napredne poizvedbe za lov

Če želite hitreje dobiti rezultate in se izogniti časovnim presledkom med izvajanjem zapletenih poizvedb, uporabite te najboljše prakse:

- Ko poskušate uporabiti nove poizvedbe, vedno uporabite omejitev, da se izognete zelo velikim naborom rezultatov. Uporabite tudi, `count` Če želite opraviti začetno oceno velikosti nabora rezultatov.
- Najprej uporabite časovne filtre. V idealnem primeru omejite svoje poizvedbe na sedem dni.
- Na začetku poizvedbe takoj za časovnim filtrom dodajte filtre, ki naj bi odstranili večino podatkov.
- Ko iščete polne žetone, uporabite `has` operator namesto `contains` .
- Zaženite iskanje v določenem stolpcu in ne v vseh stolpcih.
- Ko se pridružite tabelam, najprej določite tabelo z manj vrsticami.
- `project` le potrebne stolpce iz tabel, ki ste jih priključili.

Če želite izvedeti več, glejte [napredne prakse za lov](https://go.microsoft.com/fwlink/?linkid=2144812)na iskanje.
