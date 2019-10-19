---
title: Kako onemogočiti zunanje skupine
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739509"
---
# <a name="how-to-disable-external-groups"></a>Kako onemogočiti zunanje skupine

Za zunanje sporočanje yammer veljajo pravila Exchangeevega prenosa (ETRs), niz proaktivnih kontrolnikov, ki preprečujejo skupno rabo podatkov podjetja. Če želite uporabnikom omejiti ustvarjanje zunanjih skupin, morate konfigurirati pravilo za Exchangeeva pravila (ETR) in nato konfigurirati storitev Yammer, če želite blokirati zunanje sporočanje s pravilom Exchangevega transporta.
  
Ko ustvarite pravilo v skrbniškem središču za Exchange Online, sledite tem korakom, da nastavite ETR za uporabo v storitvi Yammer:
  
- Prijavite se v storitev Yammer kot preverjen skrbnik in v **skrbniškem središču yammer**pojdite na vsebino C **in varnostne \> varnostne nastavitve.**

- V razdelku **zunanje sporočanje** **v storitvi Yammer izberite uveljavi pravila za prenos Exchange Online Exchange (etrs).**

- Izberite **Shrani**.

Če želite več informacij, glejte [Onemogočanje zunanjega sporočanja v omrežju Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  