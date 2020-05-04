---
title: Nameščanje Officea v terminal server-brez licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010630"
---
# <a name="installing-office-on-a-terminal-server"></a>Nameščanje Officea v terminalski strežnik

Za uvajanje Microsoftovih 365 aplikacij za podjetje v operacijskem sistemu Windows Server z uporabo storitev oddaljenega namizja (RDS), prej imenovanih terminalske storitve:
  
- Imeti morate naročnino na Microsoftovo 365, ki vključuje Microsoft 365 apps za podjetje, kot je Office 365 Enterprise E3 ali Enterprise E5. Microsoft 365 Apps for Business in Microsoft 365 apps za poslovne Premium paketi ne vključujejo Microsoft 365 apps za podjetja.

- Omogočiti morate aktiviranje v [skupni rabi računalnika](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Če želite namestiti Microsoft 365 apps za podjetje na RDS iz Microsoft 365 skrbniško središče, ***ki uporablja privzete nastavitve namestitve***, uporabite naslednje korake.

> [!TIP]
> Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetje v načinu za aktiviranje v skupni rabi računalnika.
  
1. Preverite, kaj Microsoft 365 naročnino imate. [Preberite, kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Če je potrebno, preklopite na drugo naročnino na Microsoft 365. [Preberite, kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Če je Office že nameščen v strežniku RDS z uporabo katere koli druge naročnine za Microsoft 365, ga odstranite. Na primer, z tekoč v pregled svet \> uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu. Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.

4. V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 apps za podjetje](https://portal.office.com/OLS/MySoftware.aspx).

5. Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.

6. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:

1. Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit**in nato izberite v redu.

2. Izberite da, ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.

3. V urejevalniku registra dodajte vrednost niza» **Sharedcomputerlicensing** «z nastavitvijo 1 pod HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Če želite več podrobnosti o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje microsoftovih 365 aplikacij za podjetje z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi, si oglejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  