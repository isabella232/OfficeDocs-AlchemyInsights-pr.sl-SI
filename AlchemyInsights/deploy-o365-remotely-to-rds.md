---
title: Uvajanje Microsoftovih 365 aplikacij za podjetje za souporabo v skupni rabi na RDS, terminalskem strežniku ali VDI
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704721"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Uvajanje Microsoftovih 365 aplikacij za podjetje za souporabo v skupni rabi na RDS, terminalskem strežniku ali VDI

Če želite uporabiti Microsoftove 365 aplikacije za podjetja z uporabo storitev oddaljenega namizja (RDS), prej imenovane terminalske storitve:
- Imeti morate Microsoft 365 za poslovni načrt ali paket Office 365, ki vključuje Microsoftove 365 aplikacije za podjetja, na primer Office 365 Enterprise E3 ali Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 Apps for Business in Microsoft 365 Business Premium standard načrti ne vključujejo Microsoft 365 apps za podjetja.
- Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetje v načinu za aktiviranje v skupni rabi računalnika.

Če želite več informacij o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje microsoftovih 365 aplikacij za podjetje z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi:
- Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Glejte [Ponastavite stanje aktiviranja naročnine Aplikacije ogrodja Microsoft 365 za podjetja](https://go.microsoft.com/fwlink/?linkid=2109218).

Če želite namestiti Microsoft 365 apps za podjetje na RDS iz Microsoft 365 skrbniško središče, ***ki uporablja privzete nastavitve namestitve***, uporabite naslednje korake:

1.    Preverite, kakšno naročnino imate. [Naučite se kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Po potrebi preklopite na drugo naročnino. [Naučite se kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Če je Office že nameščen v strežniku RDS z uporabo drugih Microsoftovih naročnin, ga odstranite. Na primer, z tekoč v **pregled svet** > **uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu**. Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.
4.    V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 apps za podjetje](https://portal.office.com/OLS/MySoftware.aspx).
5.    Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.
6.    V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:
   1. Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite **Zaženi**. V polje Odpri vnesite **regedit**in nato izberite **v redu**.
   2. Izberite **da** , ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.
   3. V urejevalniku registra dodajte vrednost niza» **Sharedcomputerlicensing** «z nastavitvijo 1 pod HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

