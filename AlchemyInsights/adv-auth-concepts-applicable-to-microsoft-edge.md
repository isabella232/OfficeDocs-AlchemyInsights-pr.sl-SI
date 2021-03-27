---
title: Koncepti naprednega preverjanja pristnosti, ki veljajo za Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398601"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Koncepti naprednega preverjanja pristnosti, ki veljajo za Microsoft Edge

Spodaj so napredna zasnova preverjanja pristnosti, ki veljajo za Microsoft Edge:

**Proaktivno preverjanje pristnosti**

Ko omogočite pravilnik [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) bo Microsoft Edge poskusil proaktivno preveriti pristnost vpisanih uporabnikov prek Microsoftovih storitev. V rednih intervalih bo spletna storitev preverjala, ali je na voljo posodobljen manifest, ki vsebuje konfiguracijo, ki urejajo proaktivno preverjanje pristnosti.

Prednosti: Proaktivno preverjanje pristnosti omogoča preverjanje pristnosti za ključne storitve, kot je stran na novem zavihku »Office«. Če kot iskalnik uporabljate Bing, proaktivno preverjanje pristnosti izboljša učinkovitost delovanja naslovne vrstice in pomaga ustvariti rezultate iskanja, prilagojene potrebam vašega podjetja.

**Windows Hello CredUI za preverjanje pristnosti NTLM**

Če enotna prijava (SSO) ni na voljo, ko se spletno mesto poskuša vpisati v uporabnika prek mehanizma NTLM ali Negotiate, ta funkcija omogoča uporabniku skupno rabo poverilnic operacijskega sistema s tem mestom in izpolnjevanje zahtev preverjanja pristnosti z uporabo uporabniškega vmesnika Windows Hello Cred UI. Ta tok vpisa bo prikazan le v sistemu Windows 10 in le za uporabnike, ki med izzivom NTLM ali izzivom s pogajajo ne bodo dobili SSO.

**Samodejno vpisovanje s shranjenimi gesli**

Uporabniki, ki shranijo gesla v brskalniku Microsoft Edge, lahko omogočijo samodejni vpis na spletna mesta, kjer so shranili poverilnice. Uporabniki lahko vklopijo ali izklopijo to funkcijo v edge://settings/passwords, lahko pa jo konfigurirate v [pravilnikih upravitelja](https://go.microsoft.com/fwlink/?linkid=2134622) gesel.
