---
title: Pogojni dostop blokiram z napravo, ki je združljiva s predpisi
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
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037077"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Pogojni dostop blokiram z napravo, ki je združljiva s predpisi

**Zelo priporočljiva orodja**

- [Orodje za odpravljanje težav z registracijo naprave](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – celovito orodje, ki pomaga odpraviti najpogostejše težave z registracijo naprave.
- [Preskus povezljivosti za registracijo naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – orodje, s katerim zagotovite, da lahko naprava dostopa do končnih točk za registracijo naprave v sistemskem računu.
- [Skript za čiščenje naprave AZURE ad](https://github.com/mzmaili/AzureADDeviceCleanup) – orodje, ki se uporablja za iskanje in upravljanje zastarelih naprav v okolju.

Tukaj je nekaj pogostih razlogov, zakaj pogojni dostop morda ne deluje za napravo, ki je združljiva s predpisi, ali zakaj uporabniki **ne morejo** prejemati sporočila med zahtevo za vpis na organizacijski vir.

1. **Naprava ni v stanju zahtevane naprave z Mdm**:

Preverite veljavnost, da je naprava včlanjena v pooblaščenega ponudnika MDM, kot je InTune in *označena kot ustrežljiva*. Če želite več informacij o InTune, glejte ta [dokument](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Če želite boljše razumevanje skladnosti naprav in InTune, glejte [Uporaba pravilnika o skladnosti za nastavitev pravil za naprave, ki jih upravljate s funkcijo InTune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Če imate težave z vpisom naprave v programu InTune, poiščite podrobnosti o odpravljanju težav pri [odpravljanju težav pri vpisu naprave v Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Če želite dodatno podporo za intuned, ustvarite zahtevo za podporo. Če želite to narediti, obiščite [stran za InTune za pomoč in podporo](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Naprava ni združena v omrežje organizacije**:

Za dostop do organizacijskih virov mora biti naprava povezana z omrežjem organizacije, in sicer prek neposredne povezave ali navideznega zasebnega omrežja (VPN), ki se je priključil tudi na spletno izhodišče ali imenik Azure Active Directory. Če se želite pridruževanju delovni napravi v omrežje organizacije, glejte [Pridruževanje delovni napravi v omrežje organizacije](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Če želite registrirati osebno/BYOD napravo, glejte [registracija osebne naprave v omrežju organizacije](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Če želite preveriti, ali se je naprava priključila omrežju, lahko upoštevate navodila za registrirane naprave [tukaj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ali službene naprave [tukaj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Če želite poravnati težavo z omrežno povezljivostjo organizacije, spodaj navodila:

    1. Vpišite se v sistem Windows s službenim ali šolskim računom, na primer alain@contoso.com.
    2. Vzpostavite povezavo z omrežjem organizacije prek VPN ali DirectAccess.
    3. Ko vzpostavite povezavo, pritisnite tipko z **logotipom sistema Windows + L** , da zaklenete svojo napravo.
    4. Odklenite napravo s službenim ali šolskim računom in nato poskusite znova dostopati do problematičnega programa ali storitve.

Če se prikaže sporočilo o napaki, ki **ga ne morete več dobiti** , se lahko težava pojavi drugje.

3. **Operacijski sistem ni podprt**:

Zagotovite, da imate nameščeno podprto različico operacijskega sistema, vključno s temi:

- **Odjemalec sistema Windows**: Windows 7 ali novejša različica

- **Windows Server**: windows Server 2008 R2 ali novejša različica

- **MacOS**: MacOS X ali novejša različica

- **Android in IOS**: Najnovejša različica mobilnih operacijskih sistemov s sistemom Android in iOS

4. **Spletni brskalnik ni podprt**:

Spodaj najdete podprte brskalnike. Za podporo za Chrome s sistemom Windows 1703 ali novejšimi različicami je zahtevana pripona računov sistema Windows 10. Za Edge 85 + je treba uporabnika vpisati, da bo pravilno prenesel informacije o skladnosti naprave. Če želite več informacij, glejte [tukaj](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **IOS**: Microsoft Edge, InTune upravljani brskalnik, Safari
- **Android**: **Microsoft Edge**: InTune upravljani brskalnik, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **MacOS**: Chrome, Safari

**Če želite** več informacij o tem, kako lahko [tukaj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)pride do sporočil in odpravljanja težav.
