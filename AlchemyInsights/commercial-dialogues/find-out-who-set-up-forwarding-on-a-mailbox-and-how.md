---
title: Ugotovite, kdo je nastavil posredovanje v nabiralniku in kako
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483354"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ugotovite, kdo je nastavil posredovanje v nabiralniku in kako

Če je bila zunanja preusmeritev nastavljena na nabiralnik, je dejavnost revidirana kot del ukaza» cmdlet «Set-Mailbox. To storite tako, da poiščete dejavnost v dnevniku nadzora:

1. Obiščite središče za [skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Izberite  >  **iskanje dnevnika nadzora** iskanja.
    > [!NOTE]
    > Če opazite obvestilo, ki ga morate vklopiti, ga vklopite zdaj. Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli povleči podatkov iz prejšnjih datumov.
1. Prepričajte se, da je polje **dejavnosti** nastavljeno tako, da **prikaže rezultate za vse dejavnosti** (privzeto). Določite datumski obseg. Ni vam treba določiti uporabniškega imena.
1. Izberite **Išči**. Dejavnosti so prikazane v razdelku **Rezultati**.
1. Izberite **Rezultati filtra** in vnesite **nabiralnik** v polje Filter **dejavnosti** . To vrne vse dejavnosti **nabora nabiralnika** .
1. Če si želite ogledati podrobnosti, izberite dejavnost in nato izberite **več informacij**. V razdelku **Parametri** si lahko ogledate e-poštni naslov posredovanja, ki je bil nastavljen v nabiralniku. **ID** uporabnika predstavlja uporabnika, ki je nastavil zunanjo posredovanje v nabiralniku.
Če želite izvedeti več, glejte [Iskanje v dnevniku nadzora sistema Office 365 za odpravljanje pogostih scenarijev](https://go.microsoft.com/fwlink/?linkid=2103944).