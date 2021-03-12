---
title: Odpravljanje težav z nemoteno enotno prijavo (SSO) na osnovi OIDC
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
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747131"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Odpravljanje težav z nemoteno enotno prijavo (SSO) na osnovi OIDC

- Če želite izvedeti, kako dodati program, ki temelji na OIDC, v najemnika Azure, glejte [hitri zagon: nastavitev enotne prijave na osnovi OIDC (SSO) za aplikacijo v najemniku storitve Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Če želite več informacij o aplikacijah, s katerimi lahko izvedete enotno prijavo, si oglejte [razumevanje enotne prijave v OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Če želite več informacij o tem, ali želite kodo napisati z neposrednim pošiljanjem in rokovanjem s HTTP-jem ali pa uporabite knjižnico odprtokodne kode, namesto da bi uporabljali eno od naših knjižnic z odprtim virom, si oglejte [protokoli OAuth 2,0 in poverilnice za povezavo OpenID na Microsoftovi platformi Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokoli**

1. [Platforma Microsoft Identity in implicitni tok dotacije](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – definirana značilnost implicitne dotacije je ta, da so žetoni (žetoni za ID ali žetoni za dostop) vrnjeni neposredno iz končne točke/Authorize namesto v/Token končnici. To se pogosto uporablja kot del toka kode avtorizacije, in sicer v tem, kako se imenuje **» hibridni tok «– z žetonom ID-ja na/Authorize zahtevo skupaj s kodo za avtorizacijo**. V tem članku je opisano, kako program neposredno v skladu s protokolom v aplikaciji zaprosite za žetone iz storitve Azure AD.
2. [Microsoft Identity platform in OAuth 2,0 avtorizacija kode](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) za avtorizacijo – koda OAuth 2,0 dovoljenje zakonika lahko uporabite v aplikacijah, ki so nameščene v napravi, da pridobijo dostop do zaščitenih virov, kot so spletni vmesniki API. Če uporabljate Microsoftovo 2,0 platformo Identity, lahko v **mobilne in namizne aplikacije dodate vpis in API**. V tem članku je opisano, kako program neposredno v skladu s protokolom v aplikaciji uporabljate v katerem koli jeziku.
3. [Microsoft Identity platform in protokola OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – ko uporabljate povezavo» OpenID «za Microsoft Identity, lahko dodate dostop za vpis in API v programe. V tem članku je opisano, kako to naredite neodvisno od jezika in kako **pošiljate in prejemate sporočila http brez uporabe Microsoftovih odprtokodnih knjižnic**.
4. [Microsoft Identity platform in tokovne poverilnice za odjemalca oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – lahko uporabite dodelitev poverilnic odjemalca OAuth 2,0, ki je navedena v RFC 6749, včasih imenovana **OAuth**, ki je na voljo za dostop do spletnih virov, in sicer tako, da uporabite identiteto aplikacije. Ta vrsta donacije se pogosto uporablja za interakcije strežnika v strežniku, ki se morajo izvajati v ozadju, brez neposredne interakcije z uporabnikom. Te vrste programov se pogosto imenujejo **daemoni** ali **računi storitve**. V tem članku je opisano, kako program neposredno v skladu s protokolom v aplikaciji.
