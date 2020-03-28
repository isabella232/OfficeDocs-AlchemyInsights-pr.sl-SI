---
title: Ali se je odjemalec aplikacije Teams sesul?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030672"
---
# <a name="teams-client-crashing"></a>Ali se je odjemalec aplikacije Teams sesul?

Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:

- Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Prepričajte se, da so na voljo vsi [URL-ji in obsegi naslovov Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Vpišite se s svojim skrbniškim računom in preverite [Nadzorne plošče za stanje storitve](https://docs.microsoft.com/office365/enterprise/view-service-health), da preverite, ali je prišlo do propada ali razgradnje storitve.

 - Kot zadnji korak lahko poskusite počistiti predpomnilnik odjemalca Teams:

    1.  Popolnoma zaprite namiznega odjemalca za Microsoft Teams. Z desno tipko miške kliknite **Teams** iz pladnja ikon in kliknite **zaprite**ali zaženite upravitelja opravil in popolnoma uničite postopek.

    2.  Pomaknite se v razdelek »raziskovalec datotek« in vnesite%appdata%\Microsoft\teams.

    3.  Ko ste v imeniku, boste videli nekaj teh map:

         - V **Predpomnilniku aplikacije**odprite predpomnilnik in izbrišite vse datoteke na mestu predpomnilnika:%appdata%\Microsoft\ teams\application cache\cache.

        - V **Blob_storage**izbrišite vse datoteke:%appdata%\Microsoft\teams\ blob_storage.

        - V **Predpomnilniku**, izbrišite vse datoteke:%appdata%\Microsoft\teams\Cache.

        - V **Zbirkah podatkov**izbrišite vse datoteke:%appdata%\Microsoft\teams\databases.

        - V **GPUCache**izbrišite vse datoteke:%appdata%\Microsoft\teams\GPUcache.

        - V **IndexedDB**izbrišite datoteko. db:%appdata%\Microsoft\teams\IndexedDB.

        - V **Lokalno shrambo**izbrišite vse datoteke: shramba%appdata%\Microsoft\teams\Local.

        - Nazadnje, v **tmp**, izbrišite poljubno datoteko:%appdata%\Microsoft\teams\tmp.

    4. Znova zaženite odjemalca za aplikacijo Teams.
