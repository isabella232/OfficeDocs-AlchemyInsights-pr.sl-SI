---
title: Konfiguracija storitve za zagotavljanje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484044"
---
# <a name="configuring-the-provision-service"></a>Konfiguracija storitve za zagotavljanje

Za avtomatizirano omogočanje uporabe uporabnika za delo, Azure AD zahteva veljavne poverilnice, ki omogočajo, da se poveže z API-jem spletnih storitev delovnega dne. Poleg tega je na gumbu» preskusna povezava «na delovnem mestu v programu za omogočanje uporabe uporabnika preverjena tudi veljavnost, če se lahko povežete s posrednikom za omogočanje povezave do storitve Azure AD Connect, ki je povezan z domeno OGLASa.

Če portal Azure vrne napako ob shranjevanju poverilnic, upoštevajte spodnja navodila:

1. Potrdite, da ste konfigurirali uporabniški račun sistema za integracijo delovnega dne, kot je navedeno v razdelku Vadnica [Konfiguracija uporabnika integracijskega sistema v delovni dan](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Preverite, ali je storitev posrednika za omogočanje povezave s storitvijo Azure AD Connected in se izvaja v strežniku Windows Server s konzolo za upravljanje storitev. Stanje posrednika na portalu Azure lahko preverite tudi tako, da kliknete gumb ogled posrednika na mestu uporabe.
3. Zagotovite, da vnašate vrednost za polje» uporabniško ime za delovni dan «z obliko zapisa username@workday-najemnika. Če delovni dan – najemnik – ime manjka, preverjanje pristnosti delovnega dne ni uspešno.
4. Če konfigurirate integracijo z najemnikom izvajanja delovnega dne, si zapomnite načrtovane ure odmore za najemnika delovnega časa. Delovni dan je načrtovana določitvi časa za svoje najemnike izvajanja čez vikende (po navadi od petka zvečer do sobote zjutraj) in okvare povezljivosti v tem oknu odmore je znana težava, ki samodejno razreši takoj, ko so najemniki implementacije spet v spletu.
5. V redkih primerih se lahko prikaže tudi to sporočilo o napaki, če se je geslo uporabnika sistema integracije spremenilo zaradi osveževanja najemnika ali če je račun v zaklenjenem ali poteklem stanju. Preverite stanje uporabnika sistema integracije s skrbnikom delovnega dne.

Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
