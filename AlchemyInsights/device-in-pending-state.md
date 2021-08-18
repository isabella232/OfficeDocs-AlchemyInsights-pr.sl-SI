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
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330388"
---
# <a name="device-in-pending-state"></a>Naprava v stanju čakanja

**Pogoji:**

1. Če prvič nastavljate registracije naprav, preverite, ali ste pregledali uvod v upravljanje naprave v storitvi [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) v okviru katere boste dobili navodila za nadzor naprav nad imenikom Azure AD.
2. Če registrirate naprave neposredno v imeniku Azure AD [in](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) jih včlanite v Intune, morate najprej konfigurirati [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) in imeti licenco.
3. Prepričajte se, da imate dovoljenje za izvajanje operacij v imeniku Azure AD in imeniku AD na mestu uporabe. Nastavitve za registracije naprav lahko upravlja le globalni skrbnik v imeniku Azure AD. Če želite v imeniku Active Directory na mestu uporabe nastaviti samodejne registracije, morate biti skrbnik imenika Active Directory in storitev AD FS (če je na voljo).

Za hibridni postopek registracije pridruževanja imenika Azure AD morajo biti naprave v omrežju podjetja. Deluje tudi v omrežju VPN, vendar je treba to tudi izvneti. Slišali smo že stranke, ki potrebujejo pomoč pri odpravljanju težav s hibridnim postopkom registracije pridružitve Imeniku Azure AD v oddaljenih delovnih okoliščinah.

**Okolje za preverjanje pristnosti v oblaku (s sinhronizacijo oz. prepustno preverjanje pristnosti gesla za Azure AD)**

Ta postopek registracije se imenuje tudi »Sinhronizacija pridruži se«.

Tukaj je razčlenitev tega, kaj se zgodi med postopkom registracije:

1. Windows 10 odkrije zapis točke povezave storitve (SCP), ko se uporabnik prijavi v napravo.

    1. Naprava najprej poskuša pridobiti informacije o najemniku iz odjemalskega SCP-ja v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Če želite več informacij, glejte [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Če ne uspe, naprava komunicira z imenikom Active Directory na mestu uporabe in tako dobi informacije o najemniku od SCP-ja. Če želite preveriti SCP, si oglejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Opomba:** Priporočamo, da omogočite SCP v imeniku Active Directory in za začetno preverjanje veljavnosti uporabite le odjemalski SCP.

2. Windows 10 želite komunicirati z imenikom Azure AD pod sistemskim kontekstom, da bi se preverjali pristnost v zvezi z imenikom Azure AD.

    Preverite lahko, ali naprava lahko dostopa do Microsoftovih virov pod sistemskim računom, tako da uporabite skript [Test Device Registration Connectivity (Preskus povezljivosti naprave).](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 ustvari samopodpisano potrdilo in ga shrani pod predmet računalnika v imeniku Active Directory na mestu uporabe. Za to potrebujete pogled na krmilnik domene.

4. Predmet naprave s potrdilom je sinhroniziran z imenikom Azure AD prek storitve Azure AD Povezovalnik. Cikel sinhronizacije je privzeto vsakih 30 minut, vendar je to odvisno od konfiguracije storitve Azure AD Povezovalnik. Če želite več informacij, glejte ta [dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V tej fazi bi morali videti napravo zadevev stanju »Čakajoče« pod repatico naprave portala Azure Portal.

6. Ko se naslednji uporabnik prijavi v Windows 10, bo registracija dokončana.

    **Opomba:** Če uporabljate omrežje VPN, logotip/prijava pa prekine povezljivost domene, lahko registracijo sprožite ročno. To naredite tako:
    
    Težava z `dsregcmd /join` lokalnim skrbniškim pozivom ali oddaljeno prek storitve PSExec v računalniku.\
    Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Če želite več informacij o pogostih Azure Active Directory z registracijo naprave, glejte [Pogosta vprašanja o napravah.](https://docs.microsoft.com/azure/active-directory/devices/faq)
