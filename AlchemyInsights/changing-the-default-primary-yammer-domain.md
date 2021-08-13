---
title: Spreminjanje privzete domene Yammer
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
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950132"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Spreminjanje privzete/primarne domene Yammer

URL Yammer vsebuje trenutno primarno ime domene za vaše omrežje Yammer. To ime domene se morda ne bo ujemalo z imenom primarne domene v sistemu Office 365 ali Azure AD. Glede na število domen po meri, ki so bile dodane najemniku, obstajajo razlike, in ali je Yammer podprta konfiguracija (1 najemnik: 1 omrežje ali 1:1). Dokumentacija o [Yammer domenah in Officeu 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) je na voljo.

Najpogostejši razlog, zaradi katerega je nepravilna domena, je, da obstaja več Yammer omrežij in jih je treba združiti. [Z orodjem za selitev omrežja lahko združite v eno samo omrežje](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) je pomemben prvi korak. Preden začnete nastavljati primarno domeno, dokončajte ta postopek.

**Brez domen po meri**

Za nove najemnike bo privzeta domena (na primer fabrikam.onmicrosoft.com) iz najemnika uporabljena za Yammer. Primarna domena je nastavljena na yammer.com/fabrikam.onmicrosoft.com.

**Ena domena po meri**

Yammer bo samodejno izbral domeno po meri (npr. fabrikam.com) iz najemnika kot primarno domeno v Yammer. Nastavljena je na yammer.com/fabrikam.com. Ta sprememba je izvedena s storitvijo za sinhronizacijo domen in lahko začne veljati do 24 ur.

**Številne domene po meri**

Yammer ima lahko primarno domeno, ki se razlikuje od privzete domene najemnika. Ker je na voljo več domen po meri, Yammer ne poskuša ugibati pravilne domene od razpoložljivih. Če želite zahtevati, da je primarno ime domene spremenjeno na primarno domeno, ki jo želite izbrati, morate odpreti primer podpore.

**Dodatne informacije za odpravljanje težav**

V nekaterih primerih se je morda premaknilo med najemniki in storitev za sinhronizacijo domen se ni uspešno zagnala. Poleg nepravilne primarne domene lahko pride tudi do vpisa ali drugih težav. Če želite odpraviti to težavo, boste morda morali domene prestaviti v pravo omrežje s pomočjo Microsoftove podpore. Ta situacija zahteva neposredno pomoč in lahko traja nekaj časa, še posebej, če je na voljo zelo dolg seznam domenskih imen. Odpiranje primera podpore za pomoč pri odpravljanju teh vrst težav.

Ko delate s posrednikom za podporo, bodo preverili, ali so domene preverjene v najemniku pod vašim nadzorom. Če so dodane v vašega najemnika, ne da bi jih preverili zapisi DNS, lahko zahtevajo dodatna vprašanja za preverjanje glede domen. Prepričajte se, da je DNS preverjanje domen preverjeno tako, da pospeši postopek.
