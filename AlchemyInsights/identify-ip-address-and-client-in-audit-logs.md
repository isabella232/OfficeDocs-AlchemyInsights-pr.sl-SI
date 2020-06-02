---
title: Identificirajte naslov IP in odjemalca v dnevniku revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508932"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificirajte naslov IP in odjemalca v dnevniku revizij

Naslov IP, ki ustreza dejavnosti uporabnika ali skrbnika Microsoft 365, je prikazan v dnevniku revizij. Podatki o odjemalcu so tudi prijavljeni. Tukaj so koraki za identifikacijo teh informacij

1. Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/).

2. Pojdite na stran **Search**za  >  **iskanje dnevnika revizij** iskanja.

   Če ste zainteresirani za določeno dejavnost, jo izberite s seznama **dejavnosti** . Če ne, bodo vse dejavnosti vrnjene za izbranega uporabnika (privzeta nastavitev).

   **Opomba**: nekatere dejavnosti morda niso na voljo v meniju **dejavnosti** ; vendar pa bodo ti revizijski elementi vrnjeni, če je izbran **prikaz rezultatov za vse dejavnosti** (privzeta nastavitev).

3. Določite uporabniško ime v polju **Uporabniki** , izberite ustrezno časovno območje za dejavnost in kliknite **Iskanje**.

V rezultatih lahko vidite naslov IP za to dejavnost v podoknu z rezultati. Izberite zapis o reviziji, če si želite ogledati podrobne informacije v pojavnem meniju **podrobnosti** (na primer odjemalec, uporabnik, ki je izvedel dejanje itd.).

Če želite več informacij, glejte [Iskanje naslova IP računalnika, ki se uporablja za dostop do kompromitiranih računov](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
