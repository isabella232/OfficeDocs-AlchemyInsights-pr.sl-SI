---
title: Exchange PowerShell in opustitev osnovnega preverjanja pristnosti
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069260"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell in opustitev osnovnega preverjanja pristnosti

Za najnovejše informacije o tem, kako se lahko povežete z lupino Exchange Online PowerShell brez uporabe osnovnega preverjana pristnosti, [glejte tukaj](https://aka.ms/exops-docs). Modul Windows PowerShell V2 ne uporablja osnovnega preverjanja pristnosti.

Upoštevajte, da morate kljub temu omogočiti osnovno preverjanje pristnosti v odjemalskem računalniku.
Novi modul PowerShell V2 uporablja sodobno preverjanje pristnosti za vzpostavljanje povezave za omogočanje vseh ukazov »cmdlet« za V2, ki temeljijo na protokolu REST. Z ukazi »cmdlet« za V2 lahko dostopate tudi do starejših ukazov »cmdlet« za oddaljeni PowerShell (RPS), zaradi česar morate zagnati sejo oddaljenega ogrodja PowerShell. Če želite zagnati sejo RPS v računalniku s sistemom Windows, mora biti omogočeno osnovno preverjanje pristnosti WinRM v odjemalskem računalniku, čeprav modul preverja pristnost storitve z mehanizmom za sodobno preverjanje pristnosti. Cevovod osnovnega preverjanja pristnosti WinRM se uporablja za posredovanje žetonov za sodobno preverjanje pristnosti. Če je osnovno preverjanje pristnosti WinRM onemogočeno v odjemalskem računalniku, novi ukazi »cmdlet« za V2 še naprej delujejo (medtem ko starejši ukazi »cmdlet« za RPS ne delujejo več).
