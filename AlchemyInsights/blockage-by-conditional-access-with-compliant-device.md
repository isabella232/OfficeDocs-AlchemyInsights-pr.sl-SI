---
title: Pogojni dostop blokira me s skladno napravo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019164"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Pogojni dostop blokira me s skladno napravo

**Zelo priporočena orodja**

- [Orodje za odpravljanje težav z registracijo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) naprave – obsežno orodje, ki pomaga odpraviti najpogostejše težave z registracijo naprave.
- [Preskus skripta povezljivosti naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – orodje, ki se uporablja za zagotavljanje, da ima naprava dostop do končnih točk registracije naprav pod sistemskim računom.
- [Skript cleanup naprave Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – orodje, ki se uporablja za iskanje in upravljanje zastarelih naprav v vašem okolju.

Tukaj je nekaj pogostih razlogov, zakaj pogojni dostop morda ne  bo na voljo za skladno napravo ali razlog, zakaj so uporabniki prejeli sporočilo od tukaj ne morete dostopiti med zahtevo za vpis za vir organizacije.

1. **Naprava ni v zahtevanem stanju naprave z MDM:**

Preverite, ali je naprava včlanjen pri preverjenem ponudniku MDM, kot je Intune, in označena *kot skladna.* Če želite več informacij o intune, glejte ta [dokument.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Če želite bolje razumeti skladnost naprave s predpisi in storitve Intune, glejte Uporaba pravilnika o skladnosti s predpisi za nastavitev pravil za naprave, ki [jih upravljate s funkcijo Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Če imate težave z včlanijo naprave s storitvijo Intune, podrobnosti o odpravljanju težav najdete v [članku Odpravljanje težav z včlanitvi naprave v Microsoftu.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Za dodatno podporo za Intune ustvarite zahtevo za podporo. Če želite to narediti, obiščite [stran za pomoč in podporo za Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Naprava ni pridružena omrežju organizacij:**

Za dostop do virov organizacije mora biti naprava povezana z omrežjem organizacije bodisi prek neposredne povezave bodisi prek navideznega zasebnega omrežja (VPN) ter pridružena omrežju na mestu uporabe ali Azure Active Directory. Če se želite službeni napravi pridružiti omrežju organizacije, glejte Pridružite [službeni napravi v omrežje organizacije.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Če želite registrirati osebno napravo/napravo BYOD, glejte [Registracija osebne naprave v omrežju organizacije.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Če želite preveriti, ali se je naprava pridružila omrežju, upoštevajte navodila za registrirane naprave [tukaj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ali službene [naprave.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Če želite obseg težave za omrežno povezljivost z organizacijo, upoštevajte spodnja navodila:

    1. Vpišite se Windows s službeni ali šolskim računom, na primer s alain@contoso.com.
    2. Povezovalnik omrežja organizacije prek omrežja VPN ali DirectAccess.
    3. Ko je povezava vzpostavljena, pritisnite tipko **Windows in L, da** zaklenete napravo.
    4. S službeim ali šolskim računom odklenite napravo in nato poskusite znova dostopati do problematične aplikacije ali storitve.

Če se prikaže sporočilo **o napaki Tukaj ni več** mogoče do tja, je težava verjetno drugje.

3. **Operacijski sistem ni podprt:**

Prepričajte se, da imate nameščeno podprto različico operacijskega sistema, med drugim tudi:

- **Windows odjemalec:** Windows 7 ali novejša različica

- **Windows Server**: Windows Server 2008 R2 ali novejša različica

- **macOS:** macOS X ali novejša različica

- **Android in iOS:** Najnovejša različica operacijskih sistemov za mobilne naprave s sistemom Android in iOS

4. **Spletni brskalnik ni podprt:**

Spodaj poiščite podprte brskalnike. Če za Chrome uporabljate Windows 1703 ali novejše različice, je Windows 10 razširitev za račune. Za Edge 85+, mora biti uporabnik vpisan, da ustrezno prenese informacije o skladnosti naprave s predpisi. Več informacij najdete [tukaj.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1:** Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge: Intune** Managed Browser, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Več informacij o sporočilu **in** odpravljanju težav najdete [tukaj.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
