---
title: Exchange PowerShell in opustitev osnovnega preverjanja pristnosti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015705"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell in opustitev osnovnega preverjanja pristnosti

Za najnovejše informacije o tem, kako se lahko povežete z lupino Exchange Online PowerShell brez uporabe osnovnega preverjana pristnosti, [glejte tukaj](https://aka.ms/psbasicauth).

Upoštevajte, da morate kljub temu omogočiti osnovno preverjanje pristnosti v odjemalskem računalniku.
Novi modul PowerShell V2 uporablja sodobno preverjanje pristnosti za vzpostavljanje povezave za omogočanje vseh ukazov »cmdlet« za V2, ki temeljijo na protokolu REST. Z ukazi »cmdlet« za V2 lahko dostopate tudi do starejših ukazov »cmdlet« za oddaljeni PowerShell (RPS), zaradi česar morate zagnati sejo oddaljenega ogrodja PowerShell. Če želite zagnati sejo RPS v računalniku s sistemom Windows, mora biti omogočeno osnovno preverjanje pristnosti WinRM v odjemalskem računalniku, čeprav modul preverja pristnost storitve z mehanizmom za sodobno preverjanje pristnosti. Cevovod osnovnega preverjanja pristnosti WinRM se uporablja za posredovanje žetonov za sodobno preverjanje pristnosti. Če je osnovno preverjanje pristnosti WinRM onemogočeno v odjemalskem računalniku, novi ukazi »cmdlet« za V2 še naprej delujejo (medtem ko starejši ukazi »cmdlet« za RPS ne delujejo več).
