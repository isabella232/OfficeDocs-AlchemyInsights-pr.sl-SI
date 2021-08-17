---
title: Namestitev officea v terminalski strežnik – nilicencirana
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055174"
---
# <a name="installing-office-on-a-terminal-server"></a>Nameščanje Office v terminalski strežnik

Če želite uvesti Programi Microsoft 365 za podjetja v strežniku Windows z uporabo storitev oddaljenega namizja (RDS), prej imenovanih terminalske storitve:
  
- Imeti morate naročnino na Microsoft 365, ki vključuje Programi Microsoft 365 za podjetja, kot je Office 365 Enterprise E3 ali Enterprise E5. V Programi Microsoft 365 za manjša podjetja in Programi Microsoft 365 za manjša podjetja Premium paketi ne vključujejo Programi Microsoft 365 za podjetja.

- Omogočiti morate aktiviranje računalnika [v skupni rabi.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Če želite funkcijo Programi Microsoft 365 za podjetja RDS iz ***Skrbniško središče za Microsoft 365,*** ki uporablja privzete nastavitve namestitve, sledite tem korakom.

> [!TIP]
> Prav tako lahko prenesete in zaženete [Microsoft pomočnik za podporo in obnovitev,](https://aka.ms/SaRA_OfficeSCA_M365Portal) da Programi Microsoft 365 za podjetja v načinu aktiviranja računalnika v skupni rabi.
  
1. Preverite, Microsoft 365 naročnino imate. [Več o tem](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Po potrebi preklopite na drugo naročnino Microsoft 365 naročnino. [Več o tem](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Če Office strežniku RDS že nameščen s katero koli drugo naročnino Microsoft 365 naročnino, jo odstranite. Na primer tako, da se po oknu \> »Nadzorna plošča« odstranite program. Odstranite Microsoft [pomočnik za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če imate težave.

4. V strežniku RDS se vpišite v Skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Programi Microsoft 365 za podjetja](https://portal.office.com/OLS/MySoftware.aspx).

5. Ko Office, ***ne odpirajte programov*** in se ne vpišite v Office programov.

6. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:

1. Z desno tipko Windows gumb za izbiranje v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit in** izberite V redu.

2. Ko vas program pozove, ali želite urejevalniku registra dovoliti spreminjanje naprave, izberite Da.

3. V urejevalniku registra dodajte vrednost niza za **SharedComputerLicensing z** nastavitvijo 1 v razdelku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. V strežniku RDS se ***vpišite kot končni*** uporabnik in preverite, ali je aktiviranje računalnika v skupni rabi [omogočeno Programi Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Če želite več podrobnosti o pogojih, navodilih za namestitev in navodilih za prilagojene namestitve z orodjem za uvedbo sistema Office, glejte Uvajanje storitve Programi Microsoft 365 za podjetja s storitvami [oddaljenega namizja.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Če želite odpraviti napake, povezane z aktiviranjem računalnika v skupni rabi, glejte [Odpravljanje težav z aktiviranjem](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)računalnika v skupni rabi za Programi Microsoft 365 za podjetja.
  