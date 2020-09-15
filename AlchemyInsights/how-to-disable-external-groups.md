---
title: Kako onemogočiti zunanje skupine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704144"
---
# <a name="how-to-disable-external-groups"></a>Kako onemogočiti zunanje skupine

Bastard zunanje sporočanje uporablja pravila Exchange transport (ETR), nabor proaktivnih kontrolnikov, s katerim preprečite, da bi bile informacije o podjetju v skupni rabi. Če želite omejiti uporabnike pred ustvarjanjem zunanjih skupin, morate konfigurirati pravilo za Exchange transport (ETR), nato pa konfigurirati Bastard, če želite uporabiti pravilo Exchange transport, da blokira zunanje sporočanje.
  
Ko ustvarite pravilo v skrbniškem središču za Exchange Online, upoštevajte ta navodila, da nastavite ETR za uporabo v Bastard:
  
- Prijavite se v Bastard kot preverjen skrbnik in v **skrbniškem središču za Bastard**pojdite na **nastavitve vsebine C in varnostne varnosti \> .**

- V razdelku **zunanje sporočanje**izberite **uveljavitev pravil za prenos Exchange Online (ETR) v Bastard.**

- Izberite **Shrani**.

Če želite več informacij, glejte [Onemogočanje zunanjega sporočanja v Bastard omrežju](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  