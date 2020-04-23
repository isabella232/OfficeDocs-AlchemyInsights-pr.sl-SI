---
title: Kako onemogočiti zunanje skupine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720784"
---
# <a name="how-to-disable-external-groups"></a>Kako onemogočiti zunanje skupine

Za zunanje sporočanje yammer veljajo pravila Exchangeevega prenosa (ETRs), niz proaktivnih kontrolnikov, ki preprečujejo skupno rabo podatkov podjetja. Če želite uporabnikom omejiti ustvarjanje zunanjih skupin, morate konfigurirati pravilo za Exchangeeva pravila (ETR) in nato konfigurirati storitev Yammer, če želite blokirati zunanje sporočanje s pravilom Exchangevega transporta.
  
Ko ustvarite pravilo v skrbniškem središču za Exchange Online, sledite tem korakom, da nastavite ETR za uporabo v storitvi Yammer:
  
- Prijavite se v storitev Yammer kot preverjen skrbnik in v **skrbniškem središču yammer**pojdite na vsebino C **in varnostne \> varnostne nastavitve.**

- V razdelku **zunanje sporočanje** **v storitvi Yammer izberite uveljavi pravila za prenos Exchange Online Exchange (etrs).**

- Izberite **Shrani**.

Če želite več informacij, glejte [Onemogočanje zunanjega sporočanja v omrežju Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  