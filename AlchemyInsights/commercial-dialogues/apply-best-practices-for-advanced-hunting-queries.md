---
title: Uporaba najboljših praks za napredne poizvedbe za iskanje
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930149"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Uporaba najboljših praks za napredne poizvedbe za iskanje

Če želite dobiti rezultate hitreje in se izogniti časovnim omejitev med izvajanjem zapletenih poizvedb, uporabite te najboljše prakse:

- Ko poskušate nove poizvedbe, vedno uporabite omejitev, da preprečite pridobivanje izjemno velikih naborov rezultatov. Prav tako `count` se uporablja za začetno oceno velikosti nabora rezultatov.
- Najprej uporabite časovne filtre. V idealnem primeru omejite poizvedbe na sedem dni.
- Na začetku poizvedbe, takoj za časovnim filtrom, dodajte filtre, za katere ste pričakovali, da bodo odstranili večino podatkov.
- Pri iskanjem polnih žetonov uporabite `has` operator namesto `contains` .
- Namesto v vseh stolpcih zaženite iskanje v določenem stolpcu.
- Ko združujete tabele, najprej določite tabelo z manj vrsticami.
- `project` samo potrebni stolpci iz tabel, ki ste jih združili.

Če želite več informacij, glejte [Napredne prakse za poizvedbe za poizvedovanje.](https://go.microsoft.com/fwlink/?linkid=2144812)
