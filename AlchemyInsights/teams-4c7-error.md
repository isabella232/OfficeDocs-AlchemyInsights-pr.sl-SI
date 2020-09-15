---
title: Napaka» Teams 4c7 «
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700219"
---
# <a name="4c7-error-in-microsoft-teams"></a>Napaka 4c7 v aplikaciji Microsoft Teams

Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev. Ko uvedete storitve Active Directory Federation Services (AD FS), preverjanje pristnosti obrazcev privzeto ni omogočeno za intranet. Če neuspešno preverjanje pristnosti sistema Windows ni uspelo, ste pozvani k vpisu s preverjanjem pristnosti obrazcev.

Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev tako, da uporabite snap-in konzolo Microsoft Management Console (MMC) v računalniku, v katerem je lokalna kopija imenika Active Directory. Če želite to narediti, upoštevajte ta navodila: 

1. V podoknu za krmarjenje Prebrskajte do **pravilnikov o preverjanju pristnosti**.
2. V razdelku **dejanja** v podoknu s podrobnostmi izberite **Uredi globalno primarno preverjanje pristnosti**.
3. Na zavihku **intranet** izberite **preverjanje pristnosti obrazcev**.
4. Izberite **v redu** (ali **uporabi**).