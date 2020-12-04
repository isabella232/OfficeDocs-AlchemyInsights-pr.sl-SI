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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573901"
---
# <a name="troubleshoot-prt-issue"></a>Odpravljanje težav s storitvijo PRT

Za katero koli napravo, ki bo dokončana s preverjeno pristnostjo, mora biti v celoti registrirana in v dobrem stanju ter sposobna pridobiti primarni žeton za osveževanje (PRT).

Postopek registracije hibridne Azure AD JOIN zahteva, da so naprave v omrežju podjetja. Deluje tudi prek omrežja VPN, vendar je na tem mestu nekaj opozoril. Slišali smo, da stranke potrebujejo pomoč pri odpravljanju težav s procesom registracije hibridne Azure AD, ki je v skladu s pogoji oddaljenega dela. Tukaj je razčlenitev, kaj se dogaja pod kapuco med postopkom registracije.

**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo sinhronizacije z geslom Azure AD ali prepustnim preverjanjem)**

Ta potek registracije je poznan tudi kot» sinhronizacija JOIN «.

1. Windows 10 odkrije zapis SCP, ko se uporabnik prijavi v napravo.
    1. Naprava najprej poskuša pridobiti podatke najemnika na strani odjemalca SCP v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe (AD), da pridobi informacije o najemniku iz stične povezave storitve (SCP). Če želite preveriti SCP, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Priporočamo, da omogočite SCP v OGLASu in uporabljate le odjemalca SCP za začetno preverjanje veljavnosti.

2. Windows 10 poskuša komunicirati s storitvijo Azure AD v okviru sistemskega konteksta, da se preveri pristnost pred storitvijo Azure AD. Preverite lahko, ali ima naprava dostop do Microsoftovih virov v okviru sistemskega računa, in sicer tako, da uporabi skriptno povezljivost za preskusno napravo.

3. Windows 10 ustvari samopodpisano potrdilo in ga shrani pod računalnikov predmet v OGLASu na mestu uporabe. Za to morate uporabiti krmilnik domene.

4. Predmet naprave, ki ima potrdilo, je sinhroniziran s storitvijo Azure AD s povezavo» Azure AD Connect «. Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je odvisen od konfiguracije povezave s storitvijo Azure AD Connect. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Na tej stopnji lahko vidite napravo» zadeva «v razdelku» čakajoče «v razdelku» rezilo «portala Azure.

6. Pri naslednjem vpisu uporabnika v sistem Windows 10 bo registracija dokončana. 

> [!NOTE]
> Če uporabljate VPN in je postopek prijave odjave končan, lahko ročno sprožite registracijo:
 1. Izdaja dsregcmd/JOIN lokalno v skrbniškem pozivniku ali oddaljeno prek PSExec v računalnik s sistemom Windows. Na primer PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Če želite več podrobnosti o hibridnih težavah z združevanjem, glejte [Odpravljanje težav z napravami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
