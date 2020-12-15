---
title: Naprava v čakajočem stanju
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679992"
---
# <a name="device-in-pending-state"></a>Naprava v čakajočem stanju

**Predpogoji**

1. Če prvič nastavljate registracije naprav, zagotovite, da ste pregledali [Uvod v upravljanje naprav v storitvi Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , ki vas bo vodil o tem, kako pridobite naprave pod nadzorom storitve Azure ad.
2. Če želite neposredno registrirati naprave v storitvi Azure AD in jih vpisati v InTune, boste morali zagotoviti, da ste [konfigurirali InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) in imate na prvem mestu [licence](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Zagotovite, da imate dovoljenje za izvajanje operacij v storitvi Azure AD in AD na mestu uporabe. Nastavitve za registracije naprave lahko upravljajo le globalni skrbnik v storitvi Azure AD. Če želite nastaviti samodejne registracije v imeniku Active Directory na mestu uporabe, morate biti skrbnik imenika Active Directory in AD FS (po potrebi).

Postopek registracije hibridne Azure AD JOIN zahteva, da so naprave v omrežju podjetja. Deluje tudi prek omrežja VPN, vendar je na tem mestu nekaj opozoril. Slišali smo, da stranke potrebujejo pomoč pri odpravljanju težav s procesom registracije hibridne Azure AD v razdelku oddaljene delovne okoliščine.

**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo sinhronizacije z geslom Azure AD ali prepustnim preverjanjem)**

Ta potek registracije je poznan tudi kot» sinhronizacija JOIN «.

Tukaj je razdelitev tega, kaj se zgodi med postopkom registracije:

1. Windows 10 odkrije (SCP), ko se uporabnik prijavi v napravo.

    1. Naprava najprej poskuša pridobiti podatke najemnika na strani odjemalca SCP v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Če želite več informacij, glejte [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe, da pridobi informacije o najemniku iz SCP. Če želite preveriti SCP, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Priporočamo, da omogočite SCP v imeniku Active Directory in uporabljate le odjemalca SCP za začetno preverjanje veljavnosti.

2. Windows 10 poskuša komunicirati s storitvijo Azure AD v okviru sistemskega konteksta, da se preveri pristnost pred storitvijo Azure AD.

    Preverite lahko, ali ima naprava dostop do Microsoftovih virov v okviru sistemskega računa, in sicer tako, da uporabi [skriptno povezljivost za preskusno napravo](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 ustvari samopodpisano potrdilo in ga shrani pod računalnikov predmet v imeniku Active Directory na mestu uporabe. Za to morate uporabiti krmilnik domene.

4. Predmet naprave, ki ima potrdilo, je sinhroniziran s storitvijo Azure AD s povezavo» Azure AD Connect «. Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je odvisen od konfiguracije povezave s storitvijo Azure AD Connect. Če želite več informacij, si oglejte ta [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Na tej stopnji lahko vidite napravo» zadeva «v razdelku»**čakajoče**«v razdelku» rezilo «portala Azure.

6. Pri naslednjem vpisu uporabnika v sistem Windows 10 bo registracija dokončana.

    > [!NOTE]
    > Če uporabljate VPN in odjavo/prijava prekine povezljivost domene, lahko ročno sprožite registracijo. To naredite tako:
    >
    > Izdaja `dsregcmd /join` lokalno v skrbniškem pozivniku ali oddaljeno prek PSExec v računalnik s sistemom Windows.
    >
    > Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Če želite pogoste težave z registracijo naprave Azure Active Directory, glejte [pogosta vprašanja o napravah](https://docs.microsoft.com/azure/active-directory/devices/faq).
