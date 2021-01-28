---
title: Težave s terjatvami in atributi žetona
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035973"
---
# <a name="issues-with-token-claims-and-attributes"></a>Težave s terjatvami in atributi žetona

**Posodobitev, konfiguracija ali odstranitev terjatev žetona**

1. Z uporabo imenika Azure Active Directory (Azure AD) lahko [prilagodite vrsto zahtevka za zahtevek vloge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) v žetonu za odgovor, ki ga prejmete, ko pooblastite program.
2. Razvijalci aplikacij lahko v svojih aplikacijah Azure AD uporabljajo izbirne zahtevke, da določijo terjatve, ki jih želijo v žetonih, poslanih v njihovo aplikacijo. Če želite več informacij, glejte [Omogočanje izbirnih zahtevkov za vašo aplikacijo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurirajte zahteve skupine za aplikacije z imenikom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Če uporabljate nemoteno enotno prijavo v programu, glejte [prilagajanje terjatev, ki so bile izdane v SAML žetonu za podjetja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Preslikava atributov» terjatve «**

1. Če želite konfigurirati pravilnik preslikave terjatev z uporabo lupine PowerShell, glejte [prilagajanje terjatev, ki jih oddajajo žetoni za določen program v najemniku (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributi razširitve sheme Directory omogočajo shranjevanje dodatnih podatkov v imeniku Azure Active Directory na uporabniške predmete in druge predmete imenika, kot so skupine, podrobnosti najemnika, upravniki storitev. Za oddajanje zahtevkov za aplikacije lahko uporabite le atribute razširitve na uporabniških predmetih. [Z atributi pripone imeniške sheme v zahtevkih](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) je opisano, kako uporabite atribute razširitve sheme za pošiljanje uporabniških podatkov aplikacijam v žetonih.

Če želite več informacij o terjatvah žetona, glejte:

- [Terjatve v žetonih za dostop](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Terjatve v id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Terjatve](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ki jih lahko pričakujete v žetonih z ID-jem in žetonih za dostop, ki jih je izdal AZURE ad B2C
- [Sklic na SAML žetona](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
