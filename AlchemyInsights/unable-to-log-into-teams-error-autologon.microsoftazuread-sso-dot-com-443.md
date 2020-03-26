---
title: Ni se mogoče prijaviti v aplikacijo Teams zaradi napake autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932289"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Ni se mogoče prijaviti v aplikacijo Teams zaradi napake autologon.microsoftazuread-sso dot com:443

Če je za vrsto preverjanja pristnosti O365 omogočena nemotena enotna prijava, bo treba intranetnim mestom morda dodali URL »autologon.microsoftazuread-sso.com«.  Če ste ga že dodeli zaupanja vrednim spletnim mestom, nemotena enotna prijava pa je v uporabi, ga odstranite iz razdelka zaupanja vrednih mest.

Preglejte [kontrolni seznam za odpravljanje težav pri nemoteni enotni prijavi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Upoštevajte ta navodila, da dodate URL seznamu intranetnih mest:

1. Zaženite Internet Explorer tako, da kliknete gumb **Start**. V iskalno polje vnesite Internet Explorer, nato pa na seznamu rezultatov kliknite **Internet Explorer**.
2. Kliknite **Orodja** in nato **Internetne možnosti**.
3. Kliknite zavihek **Varnost**.
4. Zdaj kliknite **Lokalna intranetna mesta**, kliknite gumb **mesta** in nato še **Dodatno**.
5. Vnesite URL spletnega mesta in kliknite **Dodaj**.
6. Ko končate, kliknite **Zapri**.

Če želite več informacij, glejte [Dokumentacija za nemoteno enotno prijavo za O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (vključuje na pravilniku temelječ postopek za dodajanje URL-ja intranetnim mestom v 3. koraku).
