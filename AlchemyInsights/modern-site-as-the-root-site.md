---
title: Sodobna lokacija kot korensko mesto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666886"
---
# <a name="modern-site-as-root-site"></a>Moderno mesto kot korensko mesto

Začeli smo z uvajanjem nove funkcije, ki vam bo omogočila, da [zamenjate spletno mesto klasičnega spletnega mesta s sodobnim mestom](https://docs.microsoft.com/sharepoint/modern-root-site). Uporabite funkcijo» [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) «, da zamenjate mesto mesta z drugim mestom, medtem ko arhivirate izvirno mesto. Na voljo za spletno mesto skupine (ni povezano s skupino) in mesto za komunikacijo.

>[!Important]
> Klasičnega korenskega mesta ne izbrišite, če želite ustvariti sodobno mesto za komunikacijo. Microsoft ne podpira tega. Če izbrišete korensko mesto, bodo vsa SharePointova mesta v organizaciji nedostopna vsem uporabnikom, dokler ne obnovite mesta ali ustvarite novo mesto v istem URL-ju. To funkcijo bomo komunicirali prek središča za sporočila. Pričakujete, da bo funkcija v vašem najemniku kmalu vklopljena.

## <a name="known-issues-with-swapping-sites"></a>Znane težave s spletnimi mesti za zamenjavo
- Ciljno mesto lahko vrne napako» not found «(HTTP 404) za kratek čas.
- Vsebino bo treba znova preiskati in posodobiti indeks iskanja. Tukaj ni potrebnega ročnega koraka, to bo samodejno opravljeno.
- Vse, kar je odvisno od povezav» statičnih «(na primer sinhronizacije datotek in datotek programa OneNote), bo treba ročno popraviti.
- Če želite zagotoviti, da so še vedno pravilno povezani, je treba potrditi mesta strežnika Project Server. 
