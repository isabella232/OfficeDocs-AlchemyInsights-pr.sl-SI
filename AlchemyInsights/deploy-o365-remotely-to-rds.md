---
title: Uvajanje storitve Programi Microsoft 365 rabi v skupni rabi v rds, terminalskem strežniku ali strežniku VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077266"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Uvajanje storitve Programi Microsoft 365 rabi v skupni rabi v rds, terminalskem strežniku ali strežniku VDI

Če želite Programi Microsoft 365 uporabljati storitve oddaljenega namizja (RDS), ki so se v preteklosti imenovale terminalske storitve, morate:

- Uporabite preprost popravek, da za privzeto omogočite TLS 1.2, če uporabljate starejšo različico programa Windows (npr. Windows 7 SP1, Windows Server 2008 R2). Če želite preproste popravke in več informacij, glejte Posodobitev za omogočanje [protokola TLS 1.1 in TLS 1.2 kot](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)privzetih varnih protokolov v winhttp v brskalniku Windows. 
- Imeti morate paket, ki vključuje Programi Microsoft 365 za podjetja (prej Office 365 Plus). Na primer Office 365 E3 ali Microsoft 365 E5 ali kateri koli paket, ki vključuje namizno različico programa Project ali Visio, na primer Project (paket 3) ali Visio (paket 2), ali paket Microsoft 365 Business Premium, ki vključuje tudi Programi Microsoft 365 za manjša podjetja.
- Omogoči aktiviranje računalnika v skupni rabi. Če želite več informacij, glejte [Pregled aktiviranja računalnika v skupni rabi za Programi Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Opomba:** Če želite namestiti Programi Microsoft 365 v način aktiviranja računalnika v skupni rabi, prenesite in zaženite [Microsoft pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal). Če želite podrobnosti o pogojih, navodilih za namestitev in navodilih za prilagajanje namestitev z orodjem za uvedbo sistema Office, glejte Uvajanje storitve Programi Microsoft 365 s storitvami [oddaljenega namizja.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Če želite odpraviti napake, povezane z aktiviranjem računalnika v skupni rabi, glejte:

- [Odpravljanje težav z aktiviranjem računalnika v skupni rabi Programi Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Ponastavitev Programi Microsoft 365 za podjetja aktivacije](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Če želite podatke Programi Microsoft 365 RDS iz Skrbniško središče za Microsoft 365, ki uporablja privzete nastavitve namestitve, upoštevajte ta navodila:

1. Preverite, Microsoft 365 paket imate. Če želite več informacij, [glejte Katero naročnino imam?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Po potrebi preklopite na drug Microsoft 365 paket. Če želite več informacij, [glejte Nadgradnja na drug paket.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Če Programi Microsoft 365 strežniku RDS že nameščen s pomočjo drugih nezdružljivih paketov, jo odstranite tako, da na nadzorni plošči   >  **odstranite program.** Če na zmanjka težav, jo odstranite tako, da prenesete [Microsoft pomočnik za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. V strežniku RDS se vpišite v Skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Office](https://portal.office.com/OLS/MySoftware.aspx).

   Ko Office, ne odpirajte programov in se ne vpišite v Office programov.

1. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register:

   1. Z desno tipko miške Windows gumb za izbiranje v spodnjem levem kotu zaslona in izberite **Zaženi**. V polje Odpri vnesite **regedit in** izberite V **redu**.

   1. Ko ste pozvani, da dovolite urejevalniku registra spreminjanje naprave, izberite **Da**.

   1. V urejevalniku registra v razdelku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration dodajte vrednost niza **za SharedComputerLicensing** z nastavitvijo **1** .

1. V strežniku RDS se vpišite kot končni uporabnik in preverite, ali je aktiviranje računalnika v skupni rabi omogočeno Programi Microsoft 365. 

   Če želite več informacij, [glejte Preverjanje, ali je aktiviranje računalnika v skupni rabi omogočeno Programi Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)