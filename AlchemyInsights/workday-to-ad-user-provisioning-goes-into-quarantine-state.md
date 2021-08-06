---
title: Delovni dan za omogočanje uporabe za uporabnike AD preide v stanje karantene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036508"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Delovni dan za omogočanje uporabe za uporabnike AD preide v stanje karantene

**Delovni dan za omogočanje uporabe za uporabnike AD preide v stanje karantene in v ad se ne ustvari noben uporabnik**

Posel delovnega dne za uporabnika AD, ki omogoča uporabo, je preide v stanje karantene in dnevniki nadzora pokažejo dogodke napake pri izvozu s sporočilom o napaki **Napaka: OperationsError-SvcErr: Prišlo je do napake operacije. Za imeniško storitev ni bil konfiguriran noben nadrejeni sklic. Imeniška storitev zato ne more izdati priporočilo za predmete zunaj tega gozda.** Ta napaka se običajno prikaže, če OU vsebnika imenika Active Directory ni pravilno nastavljen ali če obstajajo težave s preslikavo izrazov, ki se uporablja za **parentDistinguishedName.**

Preverite, ali so v privzetem OU **za nove uporabnike** tipkarske napake. Prepričajte se, da navedena OU že obstaja v vašem AD-jih. Če v preslikavi atributov **uporabljate parentDistinguishedName,** zagotovite, da je vedno ovrednoteno z znanim vsebnikom znotraj domene AD. Preverite dogodek Izvozi v dnevnikih nadzora, da si ogledate ustvarjeno vrednost.

Če želite več podrobnosti o konfiguraciji delovnega dne za samodejno omogočanje uporabe, glejte Vadnica: konfiguracija delovnega [dne za samodejno omogočanje uporabe uporabnika.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

