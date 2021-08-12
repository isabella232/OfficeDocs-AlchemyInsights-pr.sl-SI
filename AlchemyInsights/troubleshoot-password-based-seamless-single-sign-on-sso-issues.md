---
title: Odpravljanje težav s nemoteno enotno prijavo na osnovi gesla
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972840"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Odpravljanje težav s nemoteno enotno prijavo na osnovi gesla

Če se želite naučiti osnove za SSO, ki temelji na geslu, glejte Preverjanje pristnosti z [geslom v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfiguracija SSO, ki temelji na geslu**

1. [Konfiguracija enotne vpise](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) na osnovi gesla – v tem članku je podrobneje opisanih možnosti enotne prijavo, ki temelji na geslu. Če aplikacija, ki jo dodajate, zahteva konfiguracijo po meri in morate uporabiti SSO, ki temelji na geslu, potem je ta članek za vas.
2. [Konfigurirajte enotno prijavo na osnovi gesla za aplikacije na mestu uporabe](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – proxy aplikacije podpira več načinov enotne prijave. Vpis z geslom je namenjen aplikacijam, ki za preverjanje pristnosti uporabljajo kombinacijo uporabniškega imena in gesla. Ko konfigurirate vpis na osnovi gesla za program, se morajo uporabniki enkrat vpisati v aplikacijo na mestu uporabe. Nato Azure Active Directory podatke za vpis in jih samodejno prikaže programu, ko uporabniki oddaljeno dostopajo do njih.
    - Aplikacijo bi morali že objaviti in preskusiti s strežnikom Application Proxy. V tem primeru upoštevajte navodila v članku Objavljanje aplikacij s strežnikom Proxy aplikacije [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) nato pa nadaljujte konfiguracijo ZSO na osnovi gesla za aplikacije na mestu uporabe.

Za odpravljanje težav s enotno prijavo na osnovi gesla si oglejte Odpravljanje težav z enotno prijavo [na podlagi gesla v imeniku Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
