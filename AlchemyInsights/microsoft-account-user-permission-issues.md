---
title: Odpravljanje težav – uporabnika ni mogoče najti v imeniku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098186"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Odpravljanje težav – uporabnika ni mogoče najti v imeniku

Če se uporabnikom v imeniku prikaže sporočilo o napaki »uporabnika ni mogoče najti«, poskusite znova, ko je vrsta težave Uporabnik ni v imeniku.

Če želite odpraviti težavo, lahko zaključite te korake.

- Prepričajte se, da je račun, ki je sprejel e-poštno povabilo, enak računu, s katerimi se boste vpisati pozneje. Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se vpiše na spletno mesto. 

Če želite več informacij, [glejte Upravljanje vzdevkov za Microsoftov račun za </a> upravljanje Microsoft 365 prijavo.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Prebrskajte do posameznih mest, na katerih uporabnik prejema napako. 

Dodajte "/_layouts/15/people.aspx/membershipgroupid=0" (znotraj dvojnih narekovajev) na konec URL-ja mesta. 

Primer: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Na seznamu izberite uporabnika.

- Na **traku kliknite Odstrani uporabniška** dovoljenja. 
-  Znova dodajte uporabnika in znova pošlji povabilo uporabniku.

