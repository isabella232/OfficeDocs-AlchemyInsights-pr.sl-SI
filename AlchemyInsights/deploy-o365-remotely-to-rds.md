---
title: Uvajanje programov Microsoft 365 za podjetja za uporabo v skupni rabi v programu RDS, Terminal Server ali VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786293"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Uvajanje programov Microsoft 365 za podjetja za uporabo v skupni rabi v programu RDS, Terminal Server ali VDI

Če želite uvesti aplikacije Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami (RDS), ki so bile prej imenovane terminalske storitve:
- Imeti morate paket Microsoft 365 za podjetja ali paket Office 365, ki vključuje aplikacije Microsoft 365 za podjetja, kot so Office 365 Enterprise E3 ali Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 apps za podjetja in Microsoft 365 Business Premium standard paketi ne vključujejo programov Microsoft 365 za podjetja.
- Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetja v načinu za aktiviranje računalnika v skupni rabi.

Če želite več informacij o predpogojih, navodilih za nastavitev in usmerjanju po prilagojenih napravah z orodjem za uvedbo sistema Office, glejte [uvajanje programov Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Odpravljanje napak, povezanih s aktiviranjem računalnika v skupni rabi:
- Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Glejte [Ponastavite stanje aktiviranja naročnine Aplikacije ogrodja Microsoft 365 za podjetja](https://go.microsoft.com/fwlink/?linkid=2109218).

Če želite namestiti aplikacije Microsoft 365 za podjetja v programu RDS v skrbniškem središču za Microsoft 365, ***ki uporablja privzete nastavitve namestitve***, uporabite te korake:

1.    Preverite, katero naročnino imate. [Preberite več o](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)tem.
2.    Po potrebi preklopite na drugo naročnino. [Preberite več o](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)tem.
3.    Če je Office že nameščen v strežniku RDS s katero koli drugo Microsoftovo naročnino, ga odstranite. Na primer, če želite **Control Panel**  >  **odstraniti program**na nadzorni plošči. Odstranite s pomočjo [Microsoftovega pomočnika za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če se izvaja težave.
4.    V strežniku RDS se vpišite v skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 aplikacije za podjetja](https://portal.office.com/OLS/MySoftware.aspx).
5.    Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove programe.
6.    V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da upoštevate te korake:
   1. Z desno tipko miške kliknite gumb sistema Windows v spodnjem levem kotu zaslona in izberite **Zaženi**. V polje Odpri vnesite **regedit**in nato izberite **v redu**.
   2. Izberite **da** , ko ste pozvani, da omogočite urejevalnik registra, da spremenite vašo napravo.
   3. V urejevalniku registra dodajte vrednost niza **SharedComputerLicensing** z nastavitvami 1 v razdelku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za programe Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

