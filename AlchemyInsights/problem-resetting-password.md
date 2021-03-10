---
title: Težava pri ponastavitvi gesla
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696278"
---
# <a name="problems-resetting-password"></a>Težave s ponastavitvijo gesla

Spodaj je navedenih nekaj težav, s katerimi se lahko soočite pri ponastavitvi gesla in možnih rešitvah:

**Imam težavo z ponastavitev gesla, ki ni zajeta v drugih kategorijah**

- Zagotovite, da imate dovoljenje za ponastavitev gesel. Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika. Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.
- Zagotovite, da razumete zahteve za licenciranje:
    - Imeti morate vsaj eno licenco, dodeljeno v organizaciji.
        - Samo uporabniki v oblaku – vsak Office 365 (O365) plačan SKU ali Azure AD Basic
        - Uporabniki v oblaku in/ali na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)
        - Če želite več informacij o zahtevah za licenciranje, si oglejte članek [zahteve za licenciranje za samopostrežno ponastavitev gesla za AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Imam težave pri testiranju pravilnika za ponastavitev gesla, ki sem ga nastavil**

- Nedavno uporabljene pravilnike lahko traja nekaj minut, da se replicirajo v vseh podatkovnih centrih in končnih točkah. Fizična razdalja od podatkovnega središča bo vplivala tudi na to, kako hitro se spremembe izvajajo.
- Preskusite s končnim uporabnikom, ne skrbnikom, in pilot z majhnim naborom uporabnikov. Pravilniki, konfigurirani v portalu Azure, veljajo le za končne uporabnike, ne skrbnike. Microsoft uveljavi močne privzete pravilnike za ponastavitev gesla za vse funkcije za skrbnike v storitvi Azure (primer: globalni skrbnik, skrbnik za pomoč, skrbnik za gesla itd.)
    - Preberite več o [pravilnikih za skrbnike](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Želim uvesti ponastavitev gesla, vendar ne želim, da moji uporabniki registrirajo dodatne varnostne informacije**

Vnaprej zapolnijo podatke za svoje uporabnike, tako da jim ni treba! -Kot skrbnik lahko nastavite lastnosti telefona in e-pošte za uporabnike pred uvajanjem ponastavitev gesla v vašo organizacijo. To lahko naredite z uporabo vmesnika API, PowerShell ali Azure AD Connect. Več informacij najdete tukaj:
- [Uvajanje ponastavitev gesla brez zahteve za registracijo uporabnikov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Katere podatke uporablja ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Gumb za ponastavitev gesla je zatemnjen**

Nimate dovoljenja za ponastavitev gesel tega uporabnika. Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika. Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.

**Rezilo za ponastavitev gesla ne vidim**

Nimate dovoljenja za ponastavitev gesel. Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika. Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.

**V ponastavitev gesla ne vidim rezila za integracijo na mestu uporabe**

- Rezilo integracije na mestu uporabe je prikazano le v hibridnih okoljih, kar pomeni, da uporabljate geslo nepotrjenim za manipuliranje uporabnikovih gesel na mestu uporabe.
- Tega rezila ne vidite, če:
    - Ne uporabljate gesla nepotrjenim
    - Prišlo je do težave z namestitvijo/povezljivostjo gesla nepotrjenim
    - Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Connect
    - Če želite več korakov za odpravljanje težav z geslom nepotrjenim, glejte razdelek [Odpravljanje težav z geslom nepotrjenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ne vem, kako ponastavim geslo uporabnika**

1. Vpišite se v portal Azure kot ustrezen skrbnik.
1. Pojdite na rezilo uporabnikov in skupin, izberite **vsi uporabniki**.
1. Izberite uporabnika s seznama.
1. Za izbranega uporabnika izberite **pregled** in nato v ukazni vrstici kliknite **Ponastavi geslo**.
1. Sledite navodilom na zaslonu.
    - Le ponastavi, izvedeno prek nepotrjenim gesla za podporo portala Azure.

**Z geslom uporabnika na mestu uporabe v skrbniškem portalu za Office 365 ali v mobilnem programu Office 365 se uporabnik še vedno ne more vpisati**

V tem portalu ni podprt Nepotrjenim za gesla. Znova ponastavite geslo uporabnika v portalu Azure – portal.azure.com

