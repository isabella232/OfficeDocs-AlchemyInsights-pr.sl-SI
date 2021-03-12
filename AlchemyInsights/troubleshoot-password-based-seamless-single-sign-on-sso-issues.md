---
title: Odpravljanje težav z nemoteno enotno prijavo (SSO), ki temelji na geslih
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714887"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Odpravljanje težav z nemoteno enotno prijavo (SSO), ki temelji na geslih

Če želite izvedeti osnove funkcije SSO, ki temelji na geslih, glejte [preverjanje pristnosti, ki temelji na geslih, z imenikom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfiguracija SSO, ki temelji na geslih**

1. [Konfiguracija enotne prijave na osnovi gesla](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – v tem članku je več podrobnosti o možnosti SSO, ki temelji na geslu. Če program, ki ga želite dodati, zahteva konfiguracijo po meri in morate uporabiti SSO, ki temelji na geslih, je ta članek za vas.
2. [Konfiguracija enotne prijave na osnovi gesla za aplikacije on-Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – aplikacija proxy podpira več načinov enotne prijave. Prijava na osnovi gesla je namenjena aplikacijam, ki uporabljajo kombinacijo uporabniškega imena in gesla za preverjanje pristnosti. Ko konfigurirate prijavo na osnovi gesla za vašo aplikacijo, se morajo uporabniki enkrat vpisati v program na mestu uporabe. V tem članku Azure Active Directory shranjuje informacije o vpisu in jih samodejno ponudi aplikaciji, ko vaši uporabniki dostopajo do njega na daljavo.
    - Aplikacijo morate že objaviti in preskusiti s proxyjem aplikacije. V nasprotnem primeru upoštevajte navodila v razdelku [objavljanje programov s proxyjem storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , nato pa nadaljujte s KONFIGURACIJO sistema SSO, ki temelji na geslu za aplikacije on-Prem.

Če želite odpraviti težave z geslom, ki temeljijo na geslu, glejte [Odpravljanje težav z enotno prijavo v storitvi AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
