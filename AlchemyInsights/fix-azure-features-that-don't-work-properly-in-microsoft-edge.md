---
title: Kaj storiti, če funkcije Azure ne delujejo pravilno v brskalniku Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583782"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Kaj storiti, če funkcije Azure ne delujejo pravilno v brskalniku Microsoft Edge

Microsoft Edge ima [znane težave](https://go.microsoft.com/fwlink/?linkid=2140608) , ki so povezane z varnostnimi območji, in lahko vpliva na to, kako se uporabniki Azure prijavijo v skrbniško središče sistema Windows. Če imate težave z uporabo funkcij Azure s programom Microsoft Edge, poskusite s temi koraki:

1. V **začetnem** meniju poiščite **Internetne možnosti** in jo izberite.
2. V pogovornem oknu **internetne lastnosti** odprite zavihek **varnost** .
3. Izberite območje **zaupanja vredna mesta** in nato izberite gumb **mesta** .
4. V pogovornem oknu **zaupanja vredna mesta** dodajte URL prehoda [https://login.microsoftonline.com](https://login.microsoftonline.com) in in [https://login.live.com](https://login.live.com) nato izberite **Zapri**.
5. V pogovornem oknu **internetne lastnosti** pojdite na zavihek **zasebnost** .
6. V razdelku **Preprečevalnik pojavnih oken** izberite **Nastavitve**. V pogovornem oknu, ki se odpre, dodajte URL prehoda, kot tudi [https://login.microsoftonline.com](https://login.microsoftonline.com) in in [https://login.live.com](https://login.live.com) nato izberite **Zapri**.
