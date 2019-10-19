---
title: Zamenjajte svojo klasično korensko stran s sodobno spletno stran
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749276"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamenjajte svojo klasično korensko stran s sodobno spletno stran

Če je bilo vaše okolje nastavljeno pred aprilom 2019, lahko korensko mesto spremenite na moderno spletno mesto z uporabo Microsoft PowerShell:

- Če imate drugačno spletno mesto, ki ga želite uporabiti kot korensko mesto, lahko z njim zamenjate [(swap) korensko mesto](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Uporaba [sklicevati-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamenjati lokacijo mesta z drugo spletno stran, medtem ko arhiviranje izvirno mesto. Na voljo za obe strani skupine (ni povezan s skupino) in mesto za komunikacijo. 

- Dodatne zmogljivosti bodo uvedene kmalu, da vam bo omogočilo, da uporabljajo vsebino na spletni strani, vendar pretvoriti obstoječe mesto na komunikacijsko mesto. 
>[!Important]
>Te zmogljivosti bodo postopoma izpeljali. Še naprej preverite Office 365 Message center za posodobitve. 

## <a name="known-issues-with-swapping-sites"></a>Znane težave s zamenjavo strani

- Ciljna stran lahko za kratek čas vrne napako» ni mogoče najti «(HTTP 404).
- Vsebino bo treba ponovno prejeti, da posodobite indeks iskanja. Ni potreben ročni korak-to se bo zgodilo samodejno.
- Vse odvisno od "statičnih" povezav (kot so file Sync in OneNote datoteke) bo treba ročno popraviti.
- Če je izvorna stran organizacijska stran z novicami, posodobite URL.Pridobite seznam vseh strani z organizacijskimi novicami.
- Mesta strežnika Project Server je morda treba potrditi, da se zagotovi, da so še vedno pravilno povezani.





