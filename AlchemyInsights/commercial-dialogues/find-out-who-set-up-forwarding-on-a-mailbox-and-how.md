---
title: Preberite, kdo je nastavil posredovanje za nabiralnik, in kako
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988228"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Preberite, kdo je nastavil posredovanje za nabiralnik, in kako

Če je bilo zunanje posredovanje nastavljeno za nabiralnik, je dejavnost nadzorovana kot del ukaza »cmdlet« Set-Mailbox»Cmdlet«. Dejavnost v dnevniku nadzora najdete tako:

1. Obiščite središče [za Office 365 za & s predpisi.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Izberite **Iskanje v** >  **dnevniku nadzora.**
    > [!NOTE]
    > Če opazite obvestilo, da morate vklopiti nadzor, ga vklopite zdaj. Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.
1. Prepričajte se, **da je** polje Dejavnosti nastavljeno **na Prikaz rezultatov za vse** dejavnosti (privzeto). Določite datumski obseg. Uporabniškega imena vam ni treba navesti.
1. Izberite **Iskanje**. Dejavnosti so prikazane v razdelku **Rezultati.**
1. Izberite **Rezultati filtriranja** in nato v **polje filter Dejavnost** vnesite **Nabiralnik** nabora. To vrne vse **dejavnosti nabiralnika nabora.**
1. Če si želite ogledati podrobnosti, izberite dejavnost, nato pa **izberite Več informacij.** V **razdelku Parametri** si lahko ogledate e-poštni naslov za posredovanje, ki je bil nastavljen za nabiralnik. ID **uporabnika** predstavlja uporabnika, ki je nastavil zunanje posredovanje za nabiralnik.
Če želite izvedeti več, [glejte Iskanje v Office 365 nadzora in odpravite pogoste scenarije.](https://go.microsoft.com/fwlink/?linkid=2103944)