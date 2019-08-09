---
title: Sodobno mesto kot korensko mesto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269392"
---
# <a name="modern-site-as-root-site"></a>Sodobno mesto kot korensko mesto

Smo začeli uvajanje novost, ki bo omogočilo, da zamenjate vaš vzoren mesto korensko mesto z moderno mesto. Uporabite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da zamenjate mesto mesto z drugim mestom med arhiviranjem na izvirno mesto. Na voljo za mesto ekipe (ne povezani skupini) in komunikacija stran. 

>[!Important]
> Ne brišite vaše klasične korensko mesto ustvariti mesto sodobne komunikacije. To je ne podpira Microsoft. Brisanje korenskega mesta bo vsa SharePointova mesta v organizaciji nedostopen za vse uporabnike, dokler obnovitev mesta ali ustvarite novo mesto na istem spletnem naslovu. Mi bomo komuniciranje lahk prek centra za sporoèila. Vi should slutiti zunanja oblika v obstati obrnjen naprej v vaš najemnik kmalu.

## <a name="known-issues-with-swapping-sites"></a>Znane težave z zamenjavo strani
- Ciljno mesto lahko vrne "not found" napaka (HTTP 404) za kratek čas.
- Vsebino morate recrawled želite posodobiti kazalo iskanja. Ni noben priročnik korak zahteva tukaj, to hoteti obstati velja automatically.
- Vse, kar je odvisno od "statična" povezave (na primer datoteka sinhronizacijo in OneNote datoteke) morali ročno popraviti.
- Projekt strežnika straneh morda morali potrditi, da se zagotovi, da so še vedno povezani pravilno. 
