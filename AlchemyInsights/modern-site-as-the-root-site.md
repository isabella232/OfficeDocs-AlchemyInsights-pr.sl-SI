---
title: Sodobno mesto kot korensko mesto
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327618"
---
# <a name="modern-site-as-root-site"></a>Sodobno mesto kot korensko mesto

Začeli smo z uvajanjem nove funkcije, ki bo omogočala zamenjavo klasičnega korenskega mesta s [sodobnim mestom](https://docs.microsoft.com/sharepoint/modern-root-site). Priklic [mesta SPOSiteSwap uporabite](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamenjavo mesta z drugim mestom med arhiviranjem izvirnega mesta. Na voljo tako za spletno mesto skupine (ni povezana s skupino) kot tudi za spletno mesto za komunikacijo.

**Pomembno:** Če želite ustvariti sodobno spletno mesto za komunikacijo, ne izbrišite klasičnega korenskega mesta. Microsoft tega ne podpira. Če izbrišete korensko mesto, bodo vsa spletna mesta SharePoint v organizaciji nedostopna za vse uporabnike, dokler ne obnovite mesta ali ustvarite novega mesta z istim URL-jem. To funkcijo bomo sporočili prek središča za sporočila. Pričakujte, da bo funkcija kmalu vklopljena v najemniku.

## <a name="known-issues-with-swapping-sites"></a>Znane težave z zamenjavo mest
- Ciljno mesto lahko za kratek čas vrne napako »ni mogoče najti« (HTTP 404).
- Če želite posodobiti kazalo iskanja, morate vsebino pretevati z pravokotno poizvedbo. Tukaj ni zahtevanih ročnih korakov, to bo narejeno samodejno.
- Vse, kar je odvisno od »statičnih« povezav (kot sta sinhronizacija datotek in OneNote), je treba ročno popraviti.
- Project Morda bo treba preveriti veljavnost spletnih mest strežnika, da se zagotovi, da so še vedno pravilno povezana. 
