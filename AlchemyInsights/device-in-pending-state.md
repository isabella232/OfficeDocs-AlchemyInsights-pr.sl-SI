---
title: Naprava v stanju čakanja
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914019"
---
# <a name="device-in-pending-state"></a>Naprava v stanju čakanja

**Pogoji:**

1. Če prvič nastavljate registracije naprav, preverite, ali ste pregledali uvod v upravljanje naprave v storitvi [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ki vas bo vodil do tega, kako zagotovite, da bodo naprave pod nadzorom imenika Azure AD.
2. Če registrirate naprave neposredno v imeniku Azure AD [in](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) jih včlanite v Intune, morate najprej konfigurirati [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) in imeti licenco.
3. Prepričajte se, da imate dovoljenje za izvajanje operacij v imeniku Azure AD in imeniku AD na mestu uporabe. Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD. Če želite v imeniku Active Directory na mestu uporabe nastaviti samodejne registracije, morate biti skrbnik imenika Active Directory in storitev AD FS (če je na voljo).

Za hibridni postopek registracije pridruževanja imenika Azure AD morajo biti naprave v omrežju podjetja. Deluje tudi v omrežju VPN, vendar obstajajo nekatere jame glede tega. Slišali smo že stranke, ki potrebujejo pomoč pri odpravljanju težav pri hibridnem postopku registracije pridružitve Imeniku Azure AD v oddaljenih delovnih okoliščinah.

**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo oz. prepustno preverjanje pristnosti gesla za Azure AD)**

Ta postopek registracije se imenuje tudi »Sinhronizacija pridruži se«.

Tukaj je razčlenitev tega, kaj se zgodi med postopkom registracije:

1. Windows 10 odkrije zapis točke povezave storitve (SCP), ko se uporabnik prijavi v napravo.

    1. Naprava najprej poskuša pridobiti informacije o najemniku iz odjemalskega SCP-ja v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Če želite več informacij, glejte [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe, da od SCP-ja dobi informacije o najemniku. Če želite preveriti SCP, si oglejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Priporočamo, da omogočite SCP v imeniku Active Directory in za začetno preverjanje veljavnosti uporabite le odjemalski SCP.

2. Windows 10 želite komunicirati z imenikom Azure AD pod sistemskim kontekstom, da bi se preverjali pristnost v imeniku Azure AD.

    Preverite lahko, ali lahko naprava dostopa do Microsoftovih virov pod sistemskim računom, tako da uporabite skript [Test Device Registration Connectivity (Preskus povezljivosti naprave).](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 ustvari samopodpisano potrdilo in ga shrani pod predmet računalnika v imeniku Active Directory na mestu uporabe. Za to potrebujete pogled na krmilnik domene.

4. Predmet naprave s potrdilom je sinhroniziran z imenikom Azure AD prek imenika Azure AD Povezovalnik. Privzeto je cikel sinhronizacije vsakih 30 minut, vendar je to odvisno od konfiguracije storitve Azure AD Povezovalnik. Če želite več informacij, glejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V tej fazi bi morali videti napravo zadevev stanju »Čakajoče« pod repatico naprave portala Azure Portal.

6. Ob prijavi naslednjega uporabnika v Windows 10, je registracija dokončana.

    > [!NOTE]
    > Če ste na omrežju VPN in logotip/prijava prekine povezljivost domene, lahko registracijo sprožite ročno. To naredite tako:
    >
    > V računalniku `dsregcmd /join` lahko težavo odpravite z lokalnim skrbniškim pozivom ali oddaljeno prek storitve PSExec.
    >
    > Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Če želite več informacij o pogostih težavah Azure Active Directory z registracijo naprave, glejte [Pogosta vprašanja o napravah.](https://docs.microsoft.com/azure/active-directory/devices/faq)
