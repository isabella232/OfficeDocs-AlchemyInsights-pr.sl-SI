---
title: Napredna koncepta preverjanja pristnosti, ki veljajo Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934381"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredna koncepta preverjanja pristnosti, ki veljajo Microsoft Edge

Spodaj so napredna koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge:

**Proaktivno preverjanje pristnosti**

Ko omogočite pravilnik [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge poskuša proaktivno preveriti pristnost vpisanih uporabnikov prek Microsoftove storitve. V rednih intervalih bo spletna storitev preverjala, ali je na voljo posodobljen manifest, ki vsebuje konfiguracijo, ki urejajo proaktivno preverjanje pristnosti.

Prednosti: Proaktivno preverjanje pristnosti omogoča preverjanje pristnosti za ključne storitve, kot Office stran na novem zavihku. Če se Bing uporablja kot mehanizem za iskanje, proaktivno preverjanje pristnosti izboljša učinkovitost delovanja naslovne vrstice in pomaga ustvariti rezultate iskanja, prilagojene potrebam vašega podjetja.

**Windows Hello CredUI za preverjanje pristnosti NTLM**

Če enotna prijava (SSO) ni na voljo, ko se spletno mesto poskuša vpisati v uporabnika prek mehanizma NTLM ali Negotiate, ta funkcija uporabniku omogoča skupno rabo poverilnic operacijskega sistema s tem mestom in izpolnjevanje zahtev preverjanja pristnosti z uporabo uporabniškega vmesnika Windows Hello Cred UI. Ta tok vpisa bo prikazan le v Windows 10 in le za uporabnike, ki med postopkom NTLM ali izzivom s pogajajo ne bodo dobili SSO.

**Samodejno vpisovanje s shranjenimi gesli**

Uporabniki, ki shranijo gesla v Microsoft Edge lahko omogočijo samodejni vpis na spletna mesta, kjer so shranili poverilnice. Uporabniki lahko vklopijo ali izklopijo to funkcijo v edge://settings/passwords, lahko pa jo konfigurirate v [pravilnikih upravitelja](https://go.microsoft.com/fwlink/?linkid=2134622) gesel.
