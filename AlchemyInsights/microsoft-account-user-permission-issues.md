---
title: Odpravljanje težav – uporabnik ni bil najden v imeniku
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768817"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Odpravljanje težav – uporabnik ni bil najden v imeniku

Če uporabnik ste sprejemanje zmota vest "uporabnik vekanje ' obstati ustanavljati" v naslovnik, prosim začeti še kraj izdaja stavek je uporabnik ne v naslovnik.

Za odpravljanje težave je mogoče dokončati naslednje korake.

- Zagotovite, da je račun, ki je sprejel e-poštno povabilo, isti račun, ki se uporablja za vpis pozneje. Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se prijavite v spletno mesto. 

Če želite več informacij, glejte [kako upravljati vzdevke za svoj Microsoftov račun</a> , da upravljate Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Prebrskajte do vsakega mesta (-ov), v katerem uporabnik prejema napako. 

Dodaj "/_layouts/15/People.aspx/membershipgroupid = 0" (znotraj dvojne narekovaje) do konca URL-ja spletnega mesta. 

Primer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Izberite uporabnika s seznama.

- Kliknite **Odstrani uporabniške pravice** s traku. 
-  Dodajte nazaj uporabnika in ponovno Pošlji povabilo uporabniku.

