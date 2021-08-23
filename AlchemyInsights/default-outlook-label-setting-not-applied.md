---
title: Privzeta nastavitev Outlook oznake ni uporabljena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455086"
---
# <a name="default-outlook-label-setting-not-applied"></a>Privzeta nastavitev Outlook oznake ni uporabljena

Če vaše privzete nastavitve oznak Outlook niso pravilno uporabljene in je uporabljena druga oznaka ali pa ni uporabljena nobena oznaka, je morda prišlo do znane težave (MC277818) in naredite eno od teh 2 možnosti, da odpravite težavo:

**1. možnost:**

1. Obiščite središče Microsoft 365 za zagotavljanje skladnosti s predpisi > **z**  >  **rešitvami za zaščito informacij.**
1. Izberite **Pravilniki za** oznake in izberite pravilnik za oznake, ki ga želite urediti ( nastavitev **OutlookDefaultlabel** ni pravilno nastavljena v pravilniku o oznakah. Zaženite **pravilnik Get-labelpolicy,** da si ogledate to nastavitev), nato pa izberite **Uredi pravilnik**.
1. Izberite **Naprej,** dokler se ne prikaže nastavitev Uporabi **to** privzeto oznako za e-pošto **,** ki je na voljo, če izberete Zahtevaj, da uporabniki v pogovornem oknu Nastavitve pravilnika uporabijo oznako za dedna  e-poštna sporočila in dokumente.
1. V pogovornem **oknu Uporabi privzeto oznako** za dokumente **na** spustnem seznamu izberite Brez.
1. Izberite **Naprej in** **Pošlji,** da shranite nastavitve nalepke.

**2. možnost:**

V [lupini Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)središča za varnost in skladnost s predpisi uporabite ukaz »Set-LabelPolicy« za spreminjanje **OutlookDefaultlabel** v **»Brez«** na {OutlookDefaultLabel="None"}.

Zaženi: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Če želite več informacij o privzetih oznakah Outlook [nalepkah, glejte Nastavitev drugačne privzete oznake za Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)