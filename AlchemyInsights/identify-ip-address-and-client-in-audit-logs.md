---
title: Prepoznavanje naslovov IP in odjemalca v dnevnikih nadzora
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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668326"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Prepoznavanje naslovov IP in odjemalca v dnevnikih nadzora

Naslov IP, ki ustreza dejavnosti, ki jo uporablja Microsoft 365 uporabnik ali skrbnik, je prikazan v dnevnikih nadzora. Podatki odjemalca so tudi prijavljeni. Tukaj so navodila za prepoznavanje teh informacij

1. Prijavite se v središče za preverjanje [varnosti & za skladnost s predpisi Microsoft 365](https://protection.office.com/).

2. Pojdite na stran **Search**  >  **iskanje dnevnika nadzora** iskanja.

   Če vas zanima določena dejavnost, jo izberite na seznamu **dejavnosti** . V nasprotnem primeru bodo vse dejavnosti vrnjene za izbranega uporabnika (privzeta nastavitev).

   **Opomba**: nekatere dejavnosti morda niso na voljo v meniju **dejavnosti** ; vendar pa bodo ti revizijski elementi vrnjeni, če je izbrana možnost **Pokaži rezultate za vse dejavnosti** (privzeta nastavitev).

3. Določite uporabniško ime v polju **Uporabniki** izberite ustrezen datumski obseg za dejavnost in nato kliknite **Išči**.

V rezultatih lahko v podoknu z rezultati vidite naslov IP za to dejavnost. Izberite zapis nadzora, če si želite ogledati podrobne informacije v flyout **podrobnosti** (na primer odjemalec, uporabnik, ki je opravil dejanje itd.).

Če želite več informacij, glejte [Iskanje naslova IP računalnika, ki se uporablja za dostop do poškodovanega računa](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
