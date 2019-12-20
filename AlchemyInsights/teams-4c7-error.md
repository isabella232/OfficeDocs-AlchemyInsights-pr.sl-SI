---
title: Napaka 4c7 ekipe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796376"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 napaka v Microsoft Teams

Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev. Ko uvedete storitve Active Directory Federation Services (AD FS), preverjanje pristnosti obrazcev ni privzeto omogočeno za intranet. Če okno enoten Authentication ne zadostovati, vi ste sufler v znamenje v using obrazec Authentication.

Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev tako, da v računalniku, v katerem je lokalna kopija imenika Active Directory, uporabite snap-in MMC konzole AD FS. Če želite to narediti, sledite tem korakom: 

1. V podoknu za krmarjenje Prebrskajte do **pravilnikov o preverjanju pristnosti**.
2. V razdelku **dejanja** v podoknu s podrobnostmi izberite **Uredi globalno primarno preverjanje pristnosti**.
3. Na zavihku **intranet** izberite **preverjanje pristnosti obrazcev**.
4. Izberite **v redu** (ali **uporabite**).