---
title: Odpravljanje težav – uporabnika ni bilo mogoče najti v imeniku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725423"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Odpravljanje težav – uporabnika ni bilo mogoče najti v imeniku

Če uporabniki prejmejo sporočilo o napaki» uporabnika ni mogoče najti «v imeniku, poskusite znova, kjer je vrsta težave uporabnik, ki ni v imeniku.

Če želite odpraviti težavo, se lahko dokončate s temi koraki.

- Zagotovite, da je račun, ki je sprejel e-poštno povabilo, isti račun, ki se uporablja za vpis pozneje. Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se vpiše na mesto. 

Če želite več informacij, glejte [upravljanje vzdevkov za Microsoftov račun </a> za upravljanje prijave v Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Poiščite vsako mesto (-e), v katerem uporabnik prejme napako. 

Dodajte»/_layouts/15/People.aspx/membershipgroupid = 0 «(znotraj dvojnih narekovajev) na konec URL-ja mesta. 

Primer: https://<» contoso «>. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Izberite uporabnika s seznama.

- Kliknite **Odstrani uporabniška dovoljenja** na traku. 
-  Dodajte uporabnika in znova pošljite povabilo uporabniku.

