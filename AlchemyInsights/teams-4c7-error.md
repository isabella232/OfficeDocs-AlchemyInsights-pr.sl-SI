---
title: Napaka »Teams 4c7«
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786685"
---
# <a name="4c7-error-in-microsoft-teams"></a>Napaka 4c7 v aplikaciji Microsoft Teams

Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev. Ko uvedete storitve AD FS (Active Directory Federation Services), preverjanje pristnosti obrazcev ni privzeto omogočeno za intranet. Če integrirano preverjanje pristnosti sistema Windows ne uspe, ste pozvani k vpisu s preverjanjem pristnosti obrazcev.

Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev s snap-inom AD FS Microsoft Management Console (MMC) v računalniku, ki ima lokalno kopijo imenika Active Directory. To naredite tako: 

1. V podoknu za krmarjenje poiščite Pravilniki **za preverjanje pristnosti.**
2. V **razdelku Dejanja** v podoknu s podrobnostmi izberite Urejanje **globalnega primarnega preverjanja pristnosti.**
3. Na zavihku **Intranet** izberite Preverjanje **pristnosti obrazcev.**
4. Izberite **V redu** (ali **Uporabi).**