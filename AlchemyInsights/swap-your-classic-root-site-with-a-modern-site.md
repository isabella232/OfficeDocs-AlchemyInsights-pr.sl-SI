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
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270760"
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





