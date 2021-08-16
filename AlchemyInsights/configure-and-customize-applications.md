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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045004"
---
# <a name="configure-and-customize-applications"></a>Konfiguracija in prilagajanje programov

**Konfiguracija programov**

1. [Hitri začetek: Konfiguriranje lastnosti programa v Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vam pokaže, kako konfigurirate nekatere lastnosti aplikacije.
2. Za integracijo programov z Azure Active Directory smo razvili [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) zbirko vadnic, ki vas bodo pomagale pri konfiguraciji.
3. [Kako konfigurirati program proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vam pomaga razumeti, kako konfigurirati program proxy aplikacije v imeniku Azure AD, da bodo aplikacije na mestu uporabe na voljo v oblaku.
4. [Prenesite PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)in konfigurirajte aplikacijo: Upoštevajte navodila v članku Konfiguracija funkcije PingAccess za *Azure AD,* da zaščitite aplikacije, objavljene s strežnikom proxy aplikacije Microsoft Azure AD na spletnem mestu Ping Identity, in prenesite najnovejšo različico funkcije PingAccess.

**Napake zaradi napačno konfigurirane aplikacije (AADSTS650056)**

1. Prepričajte se, da dostopate do programa z naslova za vpis, ki vam ga je zagotovil lastnik aplikacije. V nasprotnem primeru se vpišite v aplikacijo med običajnim postopkom. V večini primerov se bo to samodejno samodejno razrešeno naravno. Če temu ni tako, si lahko s to objavo pomagate pri odpravljanju težav.
2. **Če je vaša organizacija lastnik aplikacije** (kar pomeni, da je registracija aplikacije v vaši organizaciji):
    - Priporočamo, da dodate ali `User.Read` `openid` pooblaščeno dovoljenje družbe **Microsoft Graph** Microsoft.
    - Prepričajte se, da so za aplikacijo in vsa njena dovoljenja na voljo soglasje. To lahko preverite v stolpcu **Stanje v** razdelku Registracija aplikacije v dovoljenjih **API- ja.**
    - V nekaterih primerih je program lahko tretja oseba, vendar je morda registriran v vaši organizaciji. Preverite, ali je ta program naveden v registraciji programov (ne v poslovnih aplikacijah).
    - Če se to sporočilo o napaki še naprej prikaže. Nato boste morda morali ustvariti URL za soglasje, ki je opisan v **4. koraku.**
3. **Če vaša organizacija ni lastnik aplikacije in jo uporablja kot aplikacijo drugega ponudnika:**
    - Če ste globalni skrbnik/skrbnik podjetja, bi morali videti zaslon s soglasjem. Preverite, ali je polje **»Privolitev v imenu organizacije« potrdite.**
    - Če zaslona s soglasjem ne vidite, izbrišite aplikacijo Enterprise in poskusite znova.
    - Če se to sporočilo o napaki še naprej prikaže. Nato boste morda morali ustvariti URL za soglasje, ki je opisan v **4. koraku.**
4. Ročno **sestavljanje URL-ja** s soglasjem za uporabo: Če je aplikacija zasnovana za dostop do določenega vira, morda ne boste mogli uporabljati gumbov za soglasje na portalu Azure, boste morali ročno ustvariti svoj URL za soglasje in uporabiti ta spletni naslov.
    - Dobite aplikacijo in `{App-Id}` lastnika `{App-Uri-Id}` aplikacije. `{Tenant-Id}` bo identifikator vašega najemnika. To bo vaš `yourdomain.onmicrosoft.com` ID ali ID imenika.
    - Če program sam dostopa do vira, se isto `{App-Id}` in bo tudi v tem primeru `{App-Uri-Id}` enako.
5. Če želite več informacij, glejte Težave pri vpisu v konfigurirane aplikacije za enotno [prijavo, ki uporabljajo SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Prilagajanje programov**

- [Dodajte](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) blagovno znamko na stran za vpis v Azure Active Directory – uporabite logotip organizacije in barvne sheme po meri, da svojim stranem za vpis v Azure Active Directory (Azure AD) zagotovite dosleden videz in občutek.
- [Dodajte ime domene po meri s portalom Azure Active Directory –](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) vsak nov najemnik imenika Azure AD ima začetno ime domene. Začetnega imena domene ne morete spremeniti ali izbrisati, lahko pa dodate imena organizacije. Z dodajanjem imen domen po meri lahko ustvarite uporabniška imena, ki jih vaši uporabniki poznajo.
