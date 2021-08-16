---
title: Težave z zahtevki in atributi žetona
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012900"
---
# <a name="issues-with-token-claims-and-attributes"></a>Težave z zahtevki in atributi žetona

**Posodobitev, konfiguracija ali odstranjevanje zahtev žetona**

1. Z uporabo Azure Active Directory (Azure AD) [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) lahko prilagodite vrsto zahtevka za zahtevanje vloge v žetonu za odgovor, ki ga prejmete, ko odobrite aplikacijo.
2. Razvijalci aplikacij lahko izbirne zahtevke v aplikacijah Azure AD uporabijo za določanje, katere zahtevke želijo imeti v žetonih, poslanih v njihovo aplikacijo. Če želite več informacij, glejte [Navajajte izbirne zahtevke za aplikacijo.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurirajte zahtevke skupine za aplikacije s Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Če uporabljate nemoteno enotno prijavo v aplikaciji, glejte prilagajanje zahtevkov, izdanih v [žetonu SAML za poslovne aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Preslikava atributov zahtevkov**

1. Če želite konfigurirati pravilnik o preslikavi zahtev z lupino PowerShell, glejte Prilagajanje zahtev, izpuščenih v žetonih za določen program [v najemniku (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributi pripone sheme imenika omogočajo shranjevanje dodatnih podatkov v Azure Active Directory v uporabniške predmete in druge predmete imenika, kot so skupine, podrobnosti o najemniku, glavnice storitve. Za zahtevke za aplikacije je mogoče uporabiti le atribute pripone na uporabniških predmetih. [Uporaba atributov pripone sheme imenika v zahtevkih](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) opisuje, kako uporabiti atribute pripone sheme imenika za pošiljanje uporabniških podatkov programom v zahtevkih žetona.

Če želite več informacij o zahtevkih za žeton, glejte:

- [Zahtevki v žetonih za dostop](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Zahtevke v id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Zahtevke,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) ki jih lahko pričakujete v žetonih za ID in žetonih za dostop, ki jih je izdal Azure AD B2C
- [Sklic na zahtevke za žeton SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
