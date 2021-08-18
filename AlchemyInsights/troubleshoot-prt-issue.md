---
title: Odpravljanje težav s storitvijo PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330975"
---
# <a name="troubleshoot-prt-issue"></a>Odpravljanje težav s storitvijo PRT

Če želite, da bo vsaka naprava dokončala preverjanje pristnosti, mora biti popolnoma registrirana in v dobrem stanju ter lahko pridobi žeton za primarno osveževanje (PRT).

Za hibridni postopek registracije pridruževanja imenika Azure AD morajo biti naprave v omrežju podjetja. Deluje tudi v omrežju VPN, vendar je treba to tudi izvneti. Slišali smo, da stranke v določenih okoliščinah potrebujejo pomoč pri odpravljanju težav s hibridnim postopkom registracije pridružitve Imeniku Azure AD. Tukaj je razčlenitev tega, kaj se dogaja »pod pokrovom» med postopkom registracije.

**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo oz. prepustno preverjanje pristnosti gesla za Azure AD)**

Ta postopek registracije se imenuje tudi »Sinhronizacija pridruži se«.

1. Windows 10 zapis SCP odkrije, ko se uporabnik prijavi v napravo.
    1. Naprava najprej poskuša pridobiti informacije o najemniku iz odjemalskega SCP-ja v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Če želite več informacij, glejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe (AD), da dobi informacije o najemniku iz točke za povezavo storitve (SCP). Če želite preveriti SCP, si oglejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Opomba:** Priporočamo, da omogočite SCP v AD in za začetno preverjanje veljavnosti uporabite le odjemalski SCP.

2. Windows 10 želite komunicirati z imenikom Azure AD pod sistemskim kontekstom, da bi se preverjali pristnost v zvezi z imenikom Azure AD. Preverite lahko, ali naprava lahko dostopa do Microsoftovih virov pod sistemskim računom, tako da uporabite skript Test Device Registration Connectivity (Preskus povezljivosti naprave).

3. Windows 10 ustvari samopodpisano potrdilo in ga shrani pod računalniški predmet v AD na mestu uporabe. Za to potrebujete pogled na krmilnik domene.

4. Predmet naprave s potrdilom je sinhroniziran z imenikom Azure AD prek imenika Azure AD Povezovalnik. Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je to odvisno od konfiguracije storitve Azure AD Povezovalnik. Če želite več informacij, glejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V tej fazi bi morali videti napravo zadeve v stanju »V čakanju« v razdelku Rega naprave portala Azure Portal.

6. Ko se naslednji uporabnik prijavi v Windows 10, bo registracija dokončana. 

**Opomba:** Če uporabljate omrežje VPN in postopek prijave z logotipom prekine povezljivost domene, lahko registracijo sprožite ročno:
 1. Težavo z dsregcmd /join lokalno v skrbniškem pozivu ali oddaljeno prek storitve PSExec v računalniku. Na primer PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Če želite več podrobnosti o težavah s hibridnim pridružepom, [glejte Odpravljanje težav z napravami.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
