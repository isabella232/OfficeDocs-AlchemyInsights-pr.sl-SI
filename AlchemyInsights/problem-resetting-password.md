---
title: Težava s ponastavitvijo gesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039982"
---
# <a name="problems-resetting-password"></a>Težave s ponastavitvijo gesla

Spodaj je nekaj težav, do katerih lahko pride pri ponastavitvi gesla, in možne rešitve:

**Imam težavo s ponastavitvijo gesla, ki ni zajeta v drugih kategorijah**

- Prepričajte se, da imate dovoljenje za ponastavitev gesel. Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov. Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.
- Prepričajte se, da razumete zahteve za licenciranje:
    - V organizaciji morate imeti dodeljeno vsaj eno licenco
        - Samo uporabniki v oblaku – Office 365 inventarna številka (O365) ali Azure AD Basic
        - Uporabniki v oblaku in/ali uporabniki na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure Productive Enterprise (SPE)
        - Več informacij o zahtevah za licenciranje najdete v članku Zahteve licenciranja za [samopostrežno ponastavitev](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)gesla za Azure AD.

**Imam težave s preskušanjem pravilnika za ponastavitev gesla, ki sem ga nastavil**

- Nedavno uporabljeni pravilniki lahko trajajo nekaj minut, da se podvojite v vseh podatkovnih središčih in končnih točkah. Na to, kako hitro se spremembe uporabijo, bo vplivala tudi fizična razdalja od podatkovnega središča.
- Preskusite pri končnem uporabniku, ne skrbniku, in preskusite pri majhnem naboru uporabnikov. Pravilniki, konfigurirani na portalu Azure, veljajo LE za končne uporabnike in ne za skrbnike. Microsoft vsili močan privzeti pravilnik za ponastavitev gesla z dvema prehodoma za poljubno vlogo skrbnika azure (primer: globalni skrbnik, skrbnik središča za pomoč, skrbnik za gesla itd.)
    - Več informacij o [pravilnikih za skrbnike.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Želim uvesti ponastavitev gesla, vendar ne želim, da uporabniki registrirajo dodatne varnostne podatke**

Vnaprej napolnite podatke za uporabnike, tako da jim tega ni treba! – Kot skrbnik lahko za uporabnike nastavite lastnosti telefona in e-pošte, preden v organizaciji pošljete ponastavitev gesla. To lahko naredite z vmesnikom API, lupino PowerShell ali imenikom Azure AD Povezovalnik. Več informacij najdete tukaj:
- [Uvajanje ponastavitve gesla brez zahteve uporabnikov za registracijo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Katere podatke uporablja ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Gumb za ponastavitev gesla je zatemnjen**

Niste pooblaščeni za ponastavitev gesel tega uporabnika. Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov. Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.

**Ne vidim re bladea za ponastavitev gesla**

Niste pooblaščeni za ponastavitev gesel. Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov. Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.

**V ponastavitev gesla ne vidim re blade integracije na mestu uporabe**

- Re blade integracije na mestu uporabe se pojavi le v hibridnih okoljih – kar pomeni, da s pisanjem gesla upravljate gesla uporabnikov na mestu uporabe.
- Tega re blade ne vidite, če:
    - Ne uporabljate povratnega gesla
    - Prišlo je do težave z namestitvijo/povezljivostjo povratnega pisanja gesla
    - Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Povezovalnik
    - Če želite več korakov za odpravljanje težav s pisanjem gesla, glejte razdelek Odpravljanje [težav s pisanjem gesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ne vem, kako ponastaviti uporabnikovo geslo**

1. Vpišite se v portal Azure kot ustrezen skrbnik.
1. Pojdite na re blade Uporabniki in skupine, izberite **Vsi uporabniki.**
1. Na seznamu izberite uporabnika.
1. Za izbranega uporabnika izberite **Pregled** in nato v ukazni vrstici kliknite **Ponastavi geslo.**
1. Sledite navodilom na zaslonu.
    - Ponastavite le ponastavitve, ki jih izvedete prek portala Azure, in povratne informacije o geslih, ki jih podpira portal Azure.

**Ponastavim geslo uporabnika na mestu uporabe iz portala za Office 365 Admin ali mobilnega programa Office 365, vendar se uporabnik še vedno ne more vpisati**

Na tem portalu ni mogoče pisati gesla za pisanje gesla. Znova ponastavite geslo uporabnika na portalu Azure – portal.azure.com

