---
title: Težave s poverilnicami
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063688"
---
# <a name="issues-with-credentials"></a>Težave s poverilnicami

[Platforma Microsoft Identity in s tokom poverilnic odjemalca oauth 2,0 je](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisano, kako program neposredno v primerjavi s podelitvijo poverilnic odjemalca OAuth 2,0.

**Kako upravljam geslo ali poverilnice potrdila programa?**

V storitvi Azure CLI lahko uporabite [poverilnico programa AZ ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) , če želite izbrisati, zapisati seznam ali ponastaviti geslo za program ali poverilnice potrdila.

**Kako moji uporabniki ponastavijo gesla?**

Uporabniki se morajo [registrirati za samopostrežno ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , preden lahko ponastavijo gesla. Ko je uporabnik registriran, lahko v tem članku upoštevajo navodila za ponastavitev gesla: [ponastavitev službenega ali šolskega gesla](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kako moji uporabniki spreminjajo svoja gesla?**

Uporabniki lahko upoštevajo korake v tem članku, da spremenijo svoja gesla: [Kako spremeniti geslo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Prav tako lahko [upravljajo gesla za program za preverjanje v dveh korakih](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Moj uporabnik dobi napako pri spreminjanju ali ponastavitvi gesla**

S to povezavo boste našli informacije o pogostih težavah, ki se lahko pojavijo, ko uporabnik poskuša ponastaviti svoje geslo: [pogoste težave in njihove rešitve](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Imam težavo s ponastavitvijo uporabniškega gesla**

- Preverite, ali imate dovoljenje za ponastavitev gesel. *Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.* Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.

- Prepričajte se, da razumete zahteve za licenciranje:

  - Imeti morate vsaj eno licenco, ki je dodeljena v organizaciji:
    - **Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic
    - **Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)
    - Če želite izvedeti več o zahtevah za licenciranje, glejte [zahteve za licenciranje za samopostrežno ponastavitev gesla za storitev AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Če želite ponastaviti geslo uporabnika, poiščite uporabnika v storitvi Azure AD. Nato na rezilu pregled za tega uporabnika kliknite gumb» Ponastavi geslo «.

**Gumb za ponastavitev gesla je zatemnjen**

Nimate dovoljenja za ponastavitev gesel **tega** uporabnika. *Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.* Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.

**Rezilo za ponastavitev gesla ne vidim**

Nimate dovoljenja za ponastavitev gesel. *Gesla uporabnika lahko ponastavijo le globalni, geslo in skrbniki uporabnika.* Globalni skrbniki lahko ponastavijo tudi gesla drugih privilegiranih skrbnikov.

**V ponastavitev gesla ne vidim rezila za integracijo na mestu uporabe**

- Rezilo integracije na mestu uporabe je prikazano le v hibridnih okoljih, kar pomeni, da uporabljate geslo nepotrjenim za manipuliranje uporabnikovih gesel na mestu uporabe.

- Tega rezila ne vidite, če:

  - Ne uporabljate gesla nepotrjenim
  - Prišlo je do težave z namestitvijo/povezljivostjo gesla nepotrjenim
  - Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Connect
  - Če želite več korakov za odpravljanje težav z geslom nepotrjenim, glejte [Odpravljanje težav z geslom nepotrjenim](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne vem, kako ponastavim geslo uporabnika**

1. Vpišite se v portal Azure kot ustrezen skrbnik.
2. Pojdite na rezilo **uporabnikov in skupin** , izberite **vsi uporabniki**.
3. Izberite uporabnika s seznama.
4. Za izbranega uporabnika izberite **pregled** in nato v ukazni vrstici izberite **Ponastavi geslo**.
5. Izberite gumb za **ponastavitev gesla** in sledite navodilom na zaslonu.
    - Le ponastavi, izvedeno prek nepotrjenim gesla za podporo **portala Azure** .

**Z geslom uporabnika na mestu uporabe v skrbniškem portalu za Office 365 ali v mobilnem programu Office 365 se uporabnik še vedno ne more vpisati**

V tem portalu ni podprt Nepotrjenim za gesla. Znova ponastavite geslo uporabnika v portalu Azure.
