---
title: Prepoznavanje naslova IP in odjemalca v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887516"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje naslova IP in odjemalca v dnevnikih nadzora

Naslov IP, ki ustreza dejavnosti uporabnika ali Microsoft 365, je prikazan v dnevnikih nadzora. Zabeležene so tudi informacije o odjemalcu. Spodaj so navodila za določanje teh informacij

1. Prijavite se v središče [za Microsoft 365 s predpisi.](https://protection.office.com/)

2. Pojdite na stran **iskanja**  >  **v dnevniku nadzora** iskanja.

   Če vas zanima določena dejavnost, jo izberite na **seznamu** Dejavnosti. Če ni, bodo za izbranega uporabnika vrnjene vse dejavnosti (privzeta nastavitev).

   **Opomba:** Določene dejavnosti morda niso na voljo v **meniju** Dejavnosti. vendar pa bodo ti elementi nadzora vrnjeni, če **je izbrana možnost Pokaži rezultate** za vse dejavnosti (privzeta nastavitev).

3. V polju Uporabniki določite **uporabniško ime,** izberite ustrezen datumski obseg za dejavnost in kliknite **Išči.**

Med rezultati si lahko ogledate naslov IP za to dejavnost v podoknu z rezultati. Izberite zapis nadzora, da si  ogledate podrobne informacije v podoknu s podrobnostmi (na primer odjemalec, uporabnik, ki je izvedel dejanje itd.).

Če želite več informacij, [glejte Iskanje naslova IP računalnika, ki se uporablja za dostop do ogroženega računa.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
