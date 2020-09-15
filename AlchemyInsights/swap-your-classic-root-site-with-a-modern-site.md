---
title: Zamenjava klasičnega korenskega mesta s sodobnim mestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691195"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamenjava klasičnega korenskega mesta s sodobnim mestom

Če je bilo vaše okolje nastavljeno pred aprilom 2019, lahko korensko mesto spremenite na sodobno mesto tako, da uporabite Microsoft PowerShell:

- Če imate drugo mesto, ki ga želite uporabiti kot korensko mesto, ga lahko zamenjate [(zamenjate) s korenskim mestom](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Uporabite funkcijo» [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) «, da zamenjate mesto mesta z drugim mestom, medtem ko arhivirate izvirno mesto. Na voljo za spletno mesto skupine (ni povezano s skupino) in mesto za komunikacijo. 

- Dodatne zmogljivosti bodo kmalu predstavljene, tako da boste lahko uporabljali vsebino na spletnem mestu, vendar pretvorite obstoječe mesto na spletno mesto za komunikacijo. 
>[!Important]
>Te zmogljivosti bodo postopoma razoblikovane. Nadaljujte s preverjanjem središča za sporočila za posodobitve. 

## <a name="known-issues-with-swapping-sites"></a>Znane težave s spletnimi mesti za zamenjavo

- Ciljno mesto lahko vrne napako» not found «(HTTP 404) za kratek čas.
- Vsebino bo treba znova preiskati in posodobiti indeks iskanja. Ni potrebnega ročnega koraka – to bo samodejno opravljeno.
- Vse, kar je odvisno od povezav» statičnih «(na primer sinhronizacije datotek in datotek programa OneNote), bo treba ročno popraviti.
- Če je bilo izvorno mesto mesto organizacije novic, posodobite spletni naslov.Pridobite seznam vseh lokacij z novicami organizacije.
- Če želite zagotoviti, da so še vedno pravilno povezani, je treba potrditi mesta strežnika Project Server.
