---
title: Sodobna stran kot korensko mesto
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753920"
---
# <a name="modern-site-as-root-site"></a>Sodobna stran kot root stran

Začeli smo, da uvajanje nove funkcije, ki vam bo omogočilo, da [swap vaše klasično stran root stran s sodobno spletno stran](https://docs.microsoft.com/sharepoint/modern-root-site). Uporaba [sklicevati-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamenjati lokacijo mesta z drugo spletno stran, medtem ko arhiviranje izvirno mesto. Na voljo za obe strani skupine (ni povezan s skupino) in mesto za komunikacijo.

>[!Important]
> Ne izbrišite klasične korenske strani, da ustvarite sodobno komunikacijsko mesto. Microsoft tega ne podpira. Če izbrišete korensko mesto, bodo vsa SharePointova mesta v vaši organizaciji nedostopna vsem uporabnikom, dokler ne obnovite mesta ali ustvarite novega mesta na istem URL-ju. To funkcijo bomo komunicirali prek centra za sporočila. Pričakovati je, da bo funkcija v kratkem vklopljena v najemniku.

## <a name="known-issues-with-swapping-sites"></a>Znane težave s zamenjavo strani
- Ciljna stran lahko za kratek čas vrne napako» ni mogoče najti «(HTTP 404).
- Vsebino bo treba ponovno prejeti, da posodobite indeks iskanja. Tu ni ročnega koraka, ki je zahtevan tukaj, to se bo samodejno zgodilo.
- Vse odvisno od "statičnih" povezav (kot so file Sync in OneNote datoteke) bo treba ročno popraviti.
- Mesta strežnika Project Server je morda treba potrditi, da se zagotovi, da so še vedno pravilno povezani. 
