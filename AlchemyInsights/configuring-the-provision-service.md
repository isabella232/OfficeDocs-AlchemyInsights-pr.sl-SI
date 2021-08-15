---
title: Konfiguriranje storitve za omogočanje uporabe
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033294"
---
# <a name="configuring-the-provision-service"></a>Konfiguriranje storitve za omogočanje uporabe

Za delovanje avtomatiziranega omogočanja uporabe za uporabnike Azure AD zahteva veljavne poverilnice, ki omogočajo vzpostavitev povezave z API-jem za spletne storitve Workday. Poleg tega gumb Preskus povezave na delovnem dnevu z omogočanjem uporabe za uporabnike AD preveri tudi, ali lahko vzpostavi povezavo s posrednikom za omogočanje uporabe storitve Azure AD Povezovalnik, ki je povezan z domeno AD.

Če se portal Azure vrača napako, ko shranite poverilnice, upoštevajte priporočene korake spodaj:

1. Preverite, ali ste konfigurirali uporabniški račun sistema za integracijo delovnega dne, kot je navedeno v razdelku vadnice Konfiguracija uporabnika sistema [za integracijo v delovnem dnevu.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Preverite, ali je storitev posrednika za Povezovalnik Azure AD in se izvaja v vašem strežniku Windows mestu uporabe z uporabo konzole za upravljanje storitev. Stanje posrednika v portalu Azure lahko preverite tudi tako, da kliknete gumb Ogled posrednikov na mestu uporabe.
3. Prepričajte se, da vnašate vrednost za polje »Uporabniško ime za delovni dan« z username@workday-ime-najemnika. Če manjka ime delovnega dne-najemnika, preverjanje pristnosti delovnega dne ne uspe.
4. Če konfigurirate integracijo z najemnikom za izvedbo delavnika, si zabeležite načrtovane ure izpada najemnika delovnega dne. Delovni dan načrtuje čas izvajanja najemnikov med vikendi (ponavadi od večernega petka do sobotnega jutra) in težave s povezljivostjo v tem oknu izpada pa je znana težava, ki se samodejno razreši takoj, ko so najemniki za izvedbo znova dosegljivi.
5. V redkih primerih boste to napako morda videli tudi, če se je geslo uporabnika sistema za integracijo spremenilo zaradi osveževanja najemnika ali če je račun zaklenjen ali potekel. Preverite stanje uporabnika sistema za integracijo s skrbnikom za delovni dan.

Če želite več podrobnosti o konfiguraciji delovnega dne za samodejno omogočanje uporabe, glejte Vadnica: konfiguracija delovnega [dne za samodejno omogočanje uporabe uporabnika.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
