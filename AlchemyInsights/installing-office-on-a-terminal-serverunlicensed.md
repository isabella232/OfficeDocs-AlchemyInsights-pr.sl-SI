---
title: Nameščanje Officea v terminal server-brez licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735405"
---
# <a name="installing-office-on-a-terminal-server"></a>Nameščanje Officea v terminalski strežnik

Zakaj napotitev urad 365 ProPlus naprej a okno pomočnik using zakoten pult usluga (RDS), prej imenovan semestralen usluga:
  
- Imeti morate paket Office 365, ki vključuje Office 365 ProPlus, na primer Office 365 Enterprise E3 ali Enterprise E5. Office 365 Business in Office 365 poslovni Premium načrti ne vključujejo Office 365 ProPlus.

- Omogočiti morate aktiviranje v [skupni rabi računalnika](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Če želite namestiti Office 365 ProPlus na RDS iz Microsoft 365 skrbniškega centra, ***ki uporablja privzete nastavitve namestitve***, sledite tem korakom:
  
1. Preverite, kaj Office 365 načrt imate. [Preberite, kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Če je potrebno, preklopite na drug paket Office 365. [Preberite, kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Če je Office že nameščen v strežniku RDS z uporabo katerega koli drugega programa Office 365, ga odstranite. Na primer, z tekoč v pregled svet \> uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu. Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.

4. V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.

6. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:

1. Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit**in nato izberite v redu.

2. Izberite da, ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.

3. V registracija urednik, povečati a tetiva vrednost od **Sharedcomputerlicensing** s a postavljanje od 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Če želite več podrobnosti o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje officea 365 ProPlus z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi, glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  