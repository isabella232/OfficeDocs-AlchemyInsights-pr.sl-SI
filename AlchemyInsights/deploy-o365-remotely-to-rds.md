---
title: Uvajanje Officea 365 ProPlus za skupno uporabo na RDS, terminalskem strežniku ali VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959475"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Uvajanje Officea 365 ProPlus za skupno uporabo na RDS, terminalskem strežniku ali VDI

Če želite uvesti Office 365 ProPlus z uporabo storitev oddaljenega namizja (RDS), prej imenovane terminalske storitve:
- Imeti morate Microsoft 365 za poslovni načrt ali paket Office 365, ki vključuje Office 365 ProPlus, kot je Office 365 Enterprise E3 ali Enterprise E5.
   > [!NOTE] 
   > Office 365 Business in Office 365 poslovni Premium načrti ne vključujejo Office 365 ProPlus.
- Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Vi moči tudi travnato gričevje ter prost dostop [mikroskop zaslomba ter regres pomočnik](https://aka.ms/SaRA_OfficeSCA_M365Portal) umestiti urad 365 proplus v porazdeliti računalo activation način.

Če želite več informacij o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje officea 365 ProPlus z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi:
- Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Glej [prikrivati urad 365 ProPlus activation stanje](https://go.microsoft.com/fwlink/?linkid=2109218).

Če želite namestiti Office 365 ProPlus na RDS iz Microsoft 365 skrbniškega centra, ***ki uporablja privzete nastavitve namestitve***, uporabite naslednje korake:

1.  Preverite, kaj Office 365 načrt imate. [Naučite se kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Če je potrebno, preklopite na drug paket Office 365. [Naučite se kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Če je Office že nameščen v strežniku RDS z uporabo katerega koli drugega programa Office 365, ga odstranite. Na primer, z tekoč v **pregled svet** > **uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu**. Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.
4.  V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.
6.  V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:
   1. Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite **Zaženi**. V polje Odpri vnesite **regedit**in nato izberite **v redu**.
   2. Izberite **da** , ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.
   3. V urejevalniku registra dodajte vrednost niza» **Sharedcomputerlicensing** «z nastavitvijo 1 pod HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

