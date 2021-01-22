---
title: Nemotene težave z vpisom v uporabniškem sistemu SSO
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935182"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Nemotene težave z vpisom v uporabniškem sistemu SSO

Ko je uporabnik preverjen, bo brskalnik predpomnilnik uporabnikovih poverilnic, tako da se bo program samodejno vpisal z istim računom v istem brskalniku. Ta uporabnik ali en uporabnik lahko s tem oteži prijavo na več računov v eni napravi. Če želite odpraviti to težavo: 1. Poskusite se vpisati v drug brskalnik. 2. Odstranite predpomnilnik in/ali piškotke brskalnika in se poskusite znova vpisati.

Če imate še vedno težave z vpisom, vam priporočamo, da diagnosticirate in avtomatizirate korake resolucije:

1. Če želite v storitvi Azure Active Directory (Azure AD) za pomoč pri testiranju v portalu Azure zagotoviti boljšo diagnozo in resolucije, namestite mapo» [Moji programi «za varno razširitev brskalnika](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) .
2. Znova ustvarite napako s preskusno izkušnjo na strani s konfiguracijo aplikacije v portalu Azure. Če želite izvedeti več, glejte [debug SAML aplikacije, ki temeljijo na enotni prijavi](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Če uporabljate izkušnjo testiranja v portalu Azure s pripono varnega brskalnika My apps, lahko **preskočite korak 4**.
4. Če želite odpreti stran s konfiguracijo SAML, ki temelji na enotni strani:
    - Odprite [portal Azure](https://portal.azure.com/) in se vpišite kot **globalni skrbnik** **ali soskrbnik.**
    - Odprite **razširitev imenika Azure Active Directory** tako, da izberete **vse storitve** na vrhu glavnega menija za krmarjenje na levi strani.
    - V iskalno polje za filtriranje vnesite» Azure Active Directory «in izberite element **Azure Active Directory** .
    - V levem meniju za krmarjenje v storitvi Azure Active Directory izberite **aplikacije Enterprise** .
    - Izberite **vse aplikacije** , če si želite ogledati seznam vseh programov. Če ne vidite programa, ki ga želite prikazati tukaj, uporabite kontrolnik» **filter** «na vrhu **seznama» vsi programi** «in nastavite možnost» **Pokaži** «za **vse programe**.
    - Izberite aplikacijo, ki jo želite konfigurirati za enotno prijavo.
    - Ko se aplikacija naloži, izberite **Enotna prijava** iz levega menija za krmarjenje aplikacije.
    - Izberite **SAML, ki temelji na aplikaciji SSO**.
5. Če želite izvedeti več o priporočenih korakih, si oglejte težave z vpisom [v SAML, ki temeljijo na konfiguriranih programih enotne prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Če želite odpraviti težave z drugimi uporabniki, se obrnite na te napotke:
    - [En Sign-On SAML protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Kako: odpravljanje napak pri vpisu z uporabo poročil v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Poziv za nepričakovano privolitev](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Napaka soglasja uporabnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Težave pri vpisu iz mojih aplikacij](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Napaka na strani za vpis v program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Težave pri vpisu v Microsoftov program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
