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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986835"
---
# <a name="issues-with-credentials"></a>Težave s poverilnicami

Microsoftova platforma za identitete in tok poverilnic [odjemalca OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje, kako program neposredno v odjemalcu poverilnice OAuth 2.0 odobrijo tok.

**Kako upravljam geslo programa ali poverilnice za potrdilo?**

V storitvi Azure CLI lahko s poverilnicami za aplikacije [az ad izbrišete,](https://docs.microsoft.com/cli/azure/ad/app/credential) seznam ali ponastavite geslo aplikacije ali poverilnice za potrdilo.

**Kako uporabniki ponastavijo svoja gesla?**

Uporabniki se morajo [registrirati za samopostrežno ponastavitev gesla,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) preden lahko ponastavijo svoja gesla. Ko uporabnik registrira, lahko upošteva navodila v tem članku, da ponastavi svoje geslo: [Ponastavi vaše službeno ali šolsko geslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kako moji uporabniki spremenijo svoja gesla?**

Uporabniki lahko sledijo korakom v tem članku, če želite spremeniti svoja gesla: [Kako spremeniti geslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Prav tako lahko [upravljajo gesla za aplikacije za preverjanje v dveh korakih.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Moj uporabnik pri spreminjanju ali ponastavitvi gesla je dobival napako**

Prek te povezave so navedene informacije o pogostih težavah, do katerih lahko pride, ko uporabnik poskuša ponastaviti svoje geslo: pogoste težave in [njihove rešitve](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Imam težavo s ponastavitvijo uporabniškega gesla**

- Prepričajte se, da ste pooblaščeni za ponastavitev gesel. *Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov.* Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.

- Prepričajte se, da razumete zahteve za licenciranje:

  - V organizaciji morate imeti dodeljeno vsaj eno licenco:
    - **Samo uporabniki v oblaku** – Office 365 inventarna številka (O365) ali Azure AD Basic
    - **Uporabniki v oblaku in/ali** uporabniki na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure Productive Enterprise (SPE)
    - Če želite izvedeti več o zahtevah licenciranja, glejte [Licenčne zahteve za samopostrežno ponastavitev](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)gesla za Azure AD.
- Če želite ponastaviti geslo uporabnika, ga poiščite v imeniku Azure AD. Nato na retivu pregleda za tega uporabnika kliknite gumb »Ponastavi geslo«.

**Gumb za ponastavitev gesla je zatemnjen**

Niste pooblaščeni za **ponastavitev gesel** tega uporabnika. *Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov.* Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.

**Ne vidim re bladea za ponastavitev gesla**

Niste pooblaščeni za ponastavitev gesel. *Uporabniška gesla lahko ponastavijo le globalni skrbniki, skrbniki gesel in skrbniki uporabnikov.* Globalni skrbniki lahko ponastavijo tudi gesla drugih skrbnikov s pravicami.

**V ponastavitev gesla ne vidim re blade integracije na mestu uporabe**

- Re blade integracije na mestu uporabe se pojavi le v hibridnih okoljih – kar pomeni, da s pisanjem gesla upravljate gesla uporabnikov na mestu uporabe.

- Tega re blade ne vidite, če:

  - Ne uporabljate povratnega gesla
  - Prišlo je do težave z namestitvijo/povezljivostjo povratnega pisanja gesla
  - Prišlo je do težave z namestitvijo/povezljivostjo storitve Azure AD Povezovalnik
  - Če želite več korakov za odpravljanje težav s pisanjem gesla, glejte [Odpravljanje težav s pisanjem gesla](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne vem, kako ponastaviti uporabnikovo geslo**

1. Vpišite se v portal Azure kot ustrezen skrbnik.
2. Pojdite na re blade **Uporabniki in skupine,** izberite **Vsi uporabniki.**
3. Na seznamu izberite uporabnika.
4. Za izbranega uporabnika izberite **Pregled** in nato v ukazni vrstici izberite **Ponastavi geslo**.
5. Izberite gumb **Ponastavi geslo** in sledite navodilom na zaslonu.
    - Ponastavite le ponastavitve, ki jih **izvedete prek portala Azure,** in povratne informacije o geslih, ki jih podpira portal Azure.

**Ponastavim geslo uporabnika na mestu uporabe iz portala za Office 365 Admin ali mobilnega programa Office 365, vendar se uporabnik še vedno ne more vpisati**

Na tem portalu ni mogoče pisati gesla za pisanje gesla. Znova ponastavite geslo uporabnika na portalu Azure.
