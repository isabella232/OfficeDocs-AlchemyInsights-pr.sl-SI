---
title: Konfiguracija in prilagajanje programov
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063666"
---
# <a name="configure-and-customize-applications"></a>Konfiguracija in prilagajanje programov

**Konfiguracija programov**

1. [Hitri začetek: Konfiguracija lastnosti za program v najemniku storitve Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vam pokaže, kako konfigurirate nekatere lastnosti za program.
2. Če želite pomagati integrirati svoje aplikacije z imenikom Azure Active Directory, smo razvili [zbirko vadnic](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) , ki vas pospremijo do konfiguracije.
3. [Kako konfigurirate program proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programa, ki vam pomaga razumeti, kako konfigurirate program proxy programa v storitvi Azure ad, da razkrijete aplikacije na mestu uporabe v oblaku.
4. [Prenesite PingAccess in konfigurirajte aplikacijo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): sledite navodilom v *razdelku konfiguracija PINGACCESS za Azure ad za zaščito programov, ki* so objavljeni v aplikaciji Microsoft Azure ad proxy na spletnem mestu ping Identity in prenesite najnovejšo različico sistema PingAccess.

**Napake pri napačnem konfiguriranem programu (AADSTS650056)**

1. Zagotovite, da dostopite do programa iz naslova za vpis, ki ga je priskrbel lastnik aplikacije. V nasprotnem primeru se vpišite v aplikacijo prek običajnega postopka. V večini primerov bo to samodejno razrešilo naravno. Če se ne, lahko ta objava pomaga odpraviti težavo in jo razrešiti.
2. **Če je vaša organizacija lastnik programa** (kar pomeni, da je registracija programa v vaši organizaciji):
    - Priporočljivo je, da `User.Read` `openid` je dodana ali pooblaščeno dovoljenje za **Microsoft Graph** .
    - Zagotovite, da je program in vsa njena dovoljenja soglasna. To lahko preverite tako, da pogledate stolpec **stanje** registracije aplikacije v razdelku **dovoljenja API**.
    - V nekaterih primerih je aplikacija morda tretja oseba, vendar je morda registrirana v vaši organizaciji. Potrdite, če je ta aplikacija navedena v registracijah programov (ne v programih Enterprise).
    - Če še vedno vidite to sporočilo o napaki. Nato boste morda morali ustvariti URL za soglasje, opisan v **koraku 4**.
3. **Če vaša organizacija ni lastnik programa in jo uporablja kot program tretje osebe**:
    - Če ste skrbnik globalnega/podjetja, bi morali videti zaslon za soglasje. Prepričajte se, da potrdite polje za **» privolitev v imenu svoje organizacije «**.
    - Če ne vidite zaslona soglasja, izbrišite aplikacijo Enterprise in poskusite znova.
    - Če še vedno vidite to sporočilo o napaki. Nato boste morda morali ustvariti URL za soglasje, opisan v **koraku 4**.
4. **Ročno ustvarjanje URL-ja soglasja, ki ga želite uporabiti**: če je aplikacija zasnovana za dostop do določenega vira, morda ne boste mogli uporabljati gumbov za privolitev v portalu Azure, če želite ročno ustvariti svoj URL za soglasje in uporabiti to.
    - Lastniku aplikacije boste morali pridobiti `{App-Id}` in `{App-Uri-Id}` od njega. `{Tenant-Id}` bo identifikator najemnika. To bo bodisi `yourdomain.onmicrosoft.com` vaš ID imenika.
    - Če ima program dostop do samega vira, nato pa `{App-Id}` `{App-Uri-Id}` bo enak.
5. Če želite več informacij, glejte [težave pri vpisu v SAML, ki temeljijo na konfiguriranih programih enotne prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Prilagajanje programov**

- [Dodajanje blagovne znamke na stran za vpis](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) v storitvi Azure Active Directory v organizaciji – uporabite logotip organizacije in barvne sheme po meri, da zagotovite dosleden videz in občutek za vpisne strani v storitvi Azure Active Directory (Azure ad).
- [Dodajanje imena domene po meri z uporabo portala Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – vsak novi najemnik v storitvi Azure ad ima začetno ime domene. Prvotnega imena domene ne morete spremeniti ali izbrisati, lahko pa dodate imena organizacije. Če dodate imena domen po meri, lahko ustvarite uporabniška imena, ki jih uporabniki poznajo.
