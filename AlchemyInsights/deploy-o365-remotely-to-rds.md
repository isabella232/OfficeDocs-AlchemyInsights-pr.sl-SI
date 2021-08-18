---
title: Uvajanje storitve Programi Microsoft 365 za podjetja uporabo v skupni rabi v rds, terminalskem strežniku ali strežniku VDI
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325619"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Uvajanje storitve Programi Microsoft 365 za podjetja uporabo v skupni rabi v rds, terminalskem strežniku ali strežniku VDI

Če želite uvesti Programi Microsoft 365 za podjetja storitvami oddaljenega namizja (RDS), prej imenovanimi terminalske storitve:

- Imeti morate paket za Microsoft 365 za podjetja ali paket Office 365 ki vključuje Programi Microsoft 365 za podjetja, kot je Office 365 Enterprise E3 ali Enterprise E5.
   **Opomba:** v Programi Microsoft 365 za manjša podjetja in Microsoft 365 Business Standard paketi ne vključujejo Programi Microsoft 365 za podjetja.
- Omogočiti morate aktiviranje [računalnika v skupni rabi.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Opomba:** Lahko tudi prenesete in zaženete Microsoft [pomočnik za podporo in obnovitev, da Programi Microsoft 365 za podjetja](https://aka.ms/SaRA_OfficeSCA_M365Portal) v načinu aktiviranja računalnika v skupni rabi.

Če želite več informacij o pogojih, navodilih za namestitev in navodilih za prilagojene namestitve z orodjem za uvedbo sistema Office, glejte Uvajanje storitve Programi Microsoft 365 za podjetja s storitvami [oddaljenega namizja.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Če želite odpraviti napake, povezane z aktiviranjem računalnika v skupni rabi:

- Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Programi Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Glejte [Ponastavite stanje aktiviranja naročnine Aplikacije ogrodja Microsoft 365 za podjetja](https://go.microsoft.com/fwlink/?linkid=2109218).

Če želite funkcijo Programi Microsoft 365 za podjetja RDS iz ***Skrbniško središče za Microsoft 365,*** ki uporablja privzete nastavitve namestitve, sledite tem korakom:

1. Preverite, katero naročnino imate. [Preberite več o tem.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Po potrebi preklopite na drugo naročnino. [Preberite več o tem.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Če Office strežniku RDS že nameščen s katero koli drugo Microsoftovo naročnino, jo odstranite. Na primer, tako da se po **oknu**  >  **»Nadzorna plošča« odstranite program**. Odstranite Microsoft [pomočnik za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če imate težave.
4. V strežniku RDS se vpišite v Skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Programi Microsoft 365 za podjetja](https://portal.office.com/OLS/MySoftware.aspx).
5. Ko Office, ne ***odpirajte programov in se ne vpišite*** v Office programov.
6. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:
   1. Z desno tipko Windows gumb za izbiranje v spodnjem levem kotu zaslona in izberite **Zaženi**. V polje Odpri vnesite **regedit in** izberite V **redu**.
   2. Ko **vas program** pozove, ali želite urejevalniku registra dovoliti spreminjanje naprave, izberite Da.
   3. V urejevalniku registra dodajte vrednost niza za **SharedComputerLicensing** z nastavitvijo 1 v razdelku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. V strežniku RDS se ***vpišite kot*** končni uporabnik in preverite, ali je aktiviranje računalnika v skupni rabi [omogočeno Programi Microsoft 365 za podjetja.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
