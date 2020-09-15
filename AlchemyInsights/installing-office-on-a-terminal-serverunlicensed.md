---
title: Namestitev Officea v terminalski strežnik – brez licence
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663133"
---
# <a name="installing-office-on-a-terminal-server"></a>Namestitev Officea v terminalski strežnik

Za uvajanje programov Microsoft 365 za podjetja v sistemu Windows Server z oddaljenimi namiznimi storitvami (RDS), prej imenovanimi terminalskih storitev:
  
- Imeti morate naročnino na Microsoftovo 365, ki vključuje aplikacije Microsoft 365 za podjetja, kot so Office 365 Enterprise E3 ali Enterprise E5. Microsoft 365 apps za podjetja in Microsoft 365 apps za pakete za podjetja Premium ne vključujejo programov Microsoft 365 za podjetja.

- Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Če želite namestiti aplikacije Microsoft 365 za podjetja v programu RDS v skrbniškem središču za Microsoft 365, ***ki uporablja privzete nastavitve namestitve***, uporabite te korake.

> [!TIP]
> Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetja v načinu za aktiviranje računalnika v skupni rabi.
  
1. Preverite, katero naročnino na Microsoftovo 365 imate. [Preberite, kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Po potrebi preklopite na drugo naročnino na Microsoft 365. [Preberite, kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Če je Office že nameščen v strežniku RDS s katero koli drugo naročnino na Microsoft 365, ga odstranite. Na primer, če želite odstraniti program na nadzorni plošči \> . Odstranite s pomočjo [Microsoftovega pomočnika za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če se izvaja težave.

4. V strežniku RDS se vpišite v skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 aplikacije za podjetja](https://portal.office.com/OLS/MySoftware.aspx).

5. Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove programe.

6. V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da upoštevate te korake:

1. Z desno tipko miške kliknite gumb sistema Windows v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit**in nato izberite v redu.

2. Izberite da, ko ste pozvani, da omogočite urejevalnik registra, da spremenite vašo napravo.

3. V urejevalniku registra dodajte vrednost niza **SharedComputerLicensing** z nastavitvami 1 v razdelku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za programe Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Če želite več informacij o predpogojih, navodilih za nastavitev in usmerjanju po prilagojenih napravah z orodjem za uvedbo sistema Office, si oglejte [uvajanje programov Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Če želite odpraviti napake, povezane z aktiviranjem računalnika v skupni rabi, si oglejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  