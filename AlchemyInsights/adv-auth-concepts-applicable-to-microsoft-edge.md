---
title: Dodatni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573777"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Dodatni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge

V nadaljevanju so opisani napredni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge:

**Proaktivno preverjanje pristnosti**

Ko omogočite pravilnik o [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , bo Microsoft Edge poskušal proaktivno preveriti pristnost prijavljenih uporabnikov prek Microsoftovih storitev. V rednih časovnih presledkih bo uporaba spletne storitve za preverjanje posodobljenega manifesta, ki vsebuje konfiguracijo, ki ureja proaktivno preverjanje pristnosti.

Prednosti: proaktivno preverjanje pristnosti omogoča preverjanje pristnosti za ključne storitve, kot je na primer stran» Office New zavihek «. Če se Bing uporablja kot iskalnik, proaktivno preverjanje pristnosti izboljša učinkovitost naslovne vrstice in pomaga pri ustvarjanju rezultatov iskanja prilagojenih potrebam vašega podjetja.

**Windows hello CredUI za preverjanje pristnosti NTLM**

Če Enotna prijava (SSO) ni na voljo, ko spletno mesto poskuša podpisati uporabnika prek mehanizma NTLM ali pogajanja, bo ta funkcija uporabniku omogočila skupno rabo poverilnic OS s spletnim mestom in za zadovoljevanje preverjanja pristnosti z uporabniškim vmesnikom Windows hello verodostojnost. Ta tok za vpis bo prikazan le v sistemu Windows 10 in le za uporabnike, ki ne prejmejo SSO med NTLM ali pogajalskim izzivom.

**Uporaba shranjenih gesel za samodejno vpis**

Uporabniki, ki shranjujejo gesla v brskalniku Microsoft Edge, lahko omogočijo samodejno prijavo na spletna mesta, kjer imajo shranjene poverilnice. Uporabniki lahko to funkcijo vklopijo ali izklopijo v edge://settings/passwords, vi pa jo lahko konfigurirate v pravilnikih [upravitelja gesel](https://go.microsoft.com/fwlink/?linkid=2134622) .
