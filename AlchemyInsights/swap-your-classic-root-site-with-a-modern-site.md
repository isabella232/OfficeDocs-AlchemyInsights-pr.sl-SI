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
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940835"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamenjava klasičnega korenskega mesta s sodobnim mestom

Če je bilo vaše okolje nastavljeno pred aprilom 2019, lahko s storitvijo Microsoft PowerShell spremenite korensko mesto v sodobno mesto:

- Če imate drugo spletno mesto, ki ga želite uporabiti kot korensko mesto, zamenjajte [korensko](https://docs.microsoft.com/sharepoint/modern-root-site) mesto z njim (zamenjajte). 
    - Priklic [mesta SPOSiteSwap uporabite](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za zamenjavo mesta z drugim mestom med arhiviranjem izvirnega mesta. Na voljo tako za spletno mesto skupine (ni povezana s skupino) kot tudi za spletno mesto za komunikacijo. 

- Kmalu bodo na voljo dodatne zmogljivosti, ki bodo omogočale še naprej uporabljati vsebino mesta, vendar boste obstoječe mesto pretvorili v mesto za komunikacijo. 
>[!Important]
>Te zmogljivosti bodo postopoma na voljo. Nadaljujte s posodabljanjem v središču za sporočila. 

## <a name="known-issues-with-swapping-sites"></a>Znane težave z zamenjavo mest

- Ciljno mesto lahko za kratek čas vrne napako »ni mogoče najti« (HTTP 404).
- Za posodobitev kazala iskanja je treba vsebino oblivati z iskalno poizvedbo. Ročni korak ni potreben – to bo narejeno samodejno.
- Vse, kar je odvisno od »statičnih« povezav (kot sta sinhronizacija datotek in OneNote), je treba ročno popraviti.
- Če je bilo izvorno mesto mesto z novicami organizacije, posodobite URL. Pridobite seznam vseh spletnih mest z novicami v organizaciji.
- Project Morda bo treba preveriti veljavnost spletnih mest strežnika, da se zagotovi, da so še vedno pravilno povezana.
