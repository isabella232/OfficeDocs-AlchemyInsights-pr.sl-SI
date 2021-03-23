---
title: Pogojni dostop blokiram z napravo, ki se je priključila domeni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038103"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Pogojni dostop blokiram z napravo, ki se je priključila domeni

**Zelo priporočljiva orodja**

[Orodje za odpravljanje težav z registracijo naprave](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – orodje, ki pomaga pri odpravljanju težav najpogostejše težave pri registraciji naprave.

[Preskus povezljivosti za registracijo naprave](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, ki pomaga zagotoviti, da lahko naprava dostopa do končnih točk za registracijo naprave v sistemskem računu.

[Skript za čiščenje naprave AZURE ad](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, ki omogoča iskanje in upravljanje zastarelih naprav v okolju.

Tukaj je nekaj pogostih razlogov, zakaj pogojni dostop morda ne deluje v napravi, ki se je priključila domeni (hibridni Azure AD).

1. V **napravi ni na voljo noben oglas Azure ad prt** – morate zagotoviti, da ima naprava primarni žeton za osveževanje v storitvi Azure ad (PRT). Če želite več informacij o PRT, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Če želite preveriti, ali imate v računalniku Azure AD PRT, lahko zaženete `dsregcmd/status` ukaz v napravi in preverite, ali je» AzureAdPrt «enako» da «.

Če je» AzureAdPrt «» ne «, preverite to:

- **Ne glede na to, ali imate Združeno okolje z AD FS in je nedosegljivo iz domačih omrežij uporabnikov**: v tem primeru zagotovite, da so končne točke» usernamemixed «dostopne iz Ekstranet. Če je vaš AD FS za VPN, zagotovite, da se uporabniki povežejo z VPN in se znova prijavijo v napravo. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Ne glede na to, ali je modul zaupanja TPM okvarjen in s tem ne morete preveriti pristnosti naprave**: potrdite polje» TPM. msc «, da preverite, ali je stanje modula zaupanja TPM» Ready «. Če ne, zaženite `dsregcmd/leave` in pustite, da se naprava znova poveže s storitvijo AZURE ad. Nato poskusite znova. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Uporabljate ponudnika identitete tretje osebe, ki ne podpira WS-Trust protokola**. Kot je opisano v naših dokumentih, v tem primeru ne morejo delati hibridne naprave, ki so jih priključili v storitvi Azure AD. S ponudnikom identitete se obrnite na podporo.

2. **Uporabniki uporabljajo brskalnik Chrome brez računov Windows 10** ali sistema **Office Extension Chrome ne uporablja samodejnega** dostopa do naprav, ki so na voljo s funkcijo» neregistrirano «ali s hibridno zvočno povezavo: to privede do neuspeha vseh pravilnikov o pogojnem dostopu, ki temeljijo na napravi, in prikaže se sporočilo o napaki» Neregistrirana naprava «. Če želite uporabiti brskalnik Chrome pravilno, morate namestiti» račune sistema Windows 10 «ali» razširitev sistema Office v brskalnik Chrome za uporabnike «prek SCCM ali InTune. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Če ne morete poriniti razširitve na daljavo, obvestite uporabnike, naj ročno namestite eno od zgornjih razširitev za dostop do programov za pogojni dostop, ki temelji na napravi. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Naprava je bila pravilno hibridna AZURE ad JOIN, vendar je bila nehote izbrisana ali onemogočena, bodisi zaradi sprememb sinhronizacije v storitvi AZURE ad Connect ali iz portala Azure**: Če se to zgodi, se predmet naprave ne prepozna več kot popolnoma spojena naprava, čeprav je stanje» AzureAdJoined «in» prt «prikazano kot veljavno v napravi.

Če želite odpraviti to težavo, zaženite v `dsregcmd/leave` prizadetih napravah in jim dovolite, da se znova vključijo v AZURE ad. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Če so vaše naprave na voljo v sistemu Windows 10, 1809 Update z VPN/Cloud proxy in si ogledate težave s stanjem» AzureAdPrt «ali katero koli aplikacijo s težavo SSO (Outlook se ne poveže z nabiralnikom, čeprav ste imeli PRT), zagotovite, da imate to popravek [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ali aprilski kumulativni posodobitev [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , da preprečite okvare prt na teh strojih.

















