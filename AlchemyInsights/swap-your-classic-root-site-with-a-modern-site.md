---
title: Swap vaš Classic korensko mesto z moderno mesto
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
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246077"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap vaš Classic korensko mesto z moderno mesto

Če vaš okolja je bil ustanovljen pred aprila 2019, lahko spremenite korensko mesto na sodobno spletno stran z uporabo Microsoft PowerShell:

- Če imate drugo mesto, ki ga želite uporabiti kot korensko mesto, lahko zamenjate (swap) je koren mesto z njim. 
    - Uporabite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da zamenjate mesto mesto z drugim mestom med arhiviranjem na izvirno mesto. Na voljo za mesto ekipe (ne povezani skupini) in komunikacija stran. 

- Bo treba uvesti dodatne zmožnosti kmalu ki vam bo omogočilo, da še naprej uporabljati vsebino na mestu, ampak spremeniti obstoječega mesta na mesto komunikacije. 
>[!Important]
>Te zmogljivosti bo valjani ven postopoma. Nadaljuj, da preverite Office 365 vest središče za posodobitve. 

## <a name="known-issues-with-swapping-sites"></a>Znane težave z zamenjavo strani

- Ciljno mesto lahko vrne "not found" napaka (HTTP 404) za kratek čas.
- Vsebino morate recrawled želite posodobiti kazalo iskanja. Ni noben priročnik korak zahteva - to hoteti obstati velja automatically.
- Vse, kar je odvisno od "statična" povezave (na primer datoteka sinhronizacijo in OneNote datoteke) morali ročno popraviti.
- Če se vir organizacijske novicami, posodobite URL.Dobili seznam vseh organizacijskih novicami.
- Projekt strežnika straneh morda morali potrditi, da se zagotovi, da so še vedno povezani pravilno.





