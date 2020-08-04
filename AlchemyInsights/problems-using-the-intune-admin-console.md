---
title: Težave z uporabo skrbniške konzole Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555878"
---
# <a name="problems-using-the-intune-admin-console"></a>Težave z uporabo skrbniške konzole Intune

**»Dostop zavrnjen« pri krmarjenju po skrbniškem portalu Intune.**

- Če ste član vloge po meri Intune, se prepričajte, da je licenca EMS (Intune ali Enterprise Mobility Suite) dodeljena vašemu računu.
- Če za upravljanje naprav uporabljate upravitelja konfiguracije, preverite, ali niste del uporabniške zbirke Intune za MDM upravitelja konfiguracije.
- Preverite, ali so vam bila v rezilu »Vloge Intune« dodeljena ustrezna dovoljenja za nadzor skrbništva na podlagi vlog (RBAC).
- Preverite, ali uporabljena skupina ni seznam prejemnikov. Intune v portalu Azure podpira samo uporabniške račune, ki pripadajo varnostnim skupinam storitve Azure Active Directory. Preglejte skupine v portalu Azure > **Intune**  >  **Groups**ali v portalu Azure > **imeniku Azure Active Directory**.

**Uporabnik ima preveč dovoljenj za dodeljeno vlogo Intune**

Svetujte uporabniku, da gre **v vloge Intune**  >  **Intune**  >  **Moja dovoljenja**  >  **Izvozi,** da pregleda odobrena dovoljenja.

**Vlogi sem dodal skupino obsegov, vendar uporabniki v tej vlogi še vedno vidijo druge uporabnike ali naprave.**

Skupine obsega ne filtrirajo uporabnikov ali naprav. Skupine obsegov:

- Omejite, komu lahko uporabniki dodelijo pravilnike ali aplikacije.
- Dovoli samo določenim uporabnikom, da izvajajo oddaljena opravila v napravah.

Če želite več informacij o skupinah obsega, [glejte Nadzor dostopa do vlog (RBAC) z Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Dodal sem uporabnika intune vlogo, vendar so še vedno popoln dostop do intune admin konzolo.**

Pomaknite se do možnosti Intune > **Uporabniki** v portalu Azure in preverite, ali uporabnik ni dodeljen nobeni od teh vlog v portalu Azure:

- Globalni skrbnik
- Skrbnik storitve Intune
- Skrbnik SharePointa

Če želite več informacij, [glejte Nadzor dostopa po vlogi (RBAC) z MicrosoftOm Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Težave z dostopom**

Če želite več informacij, [glejte Ne morete se vpisati v Office 365, Azure ali Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).