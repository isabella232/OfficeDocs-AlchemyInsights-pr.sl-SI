---
title: Napeljati urad v terminalski strežnik - brez licence
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
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381745"
---
# <a name="installing-office-on-a-terminal-server"></a>Namestite Office v terminalskem strežniku

Za uvajanje Office 365 ProPlus strežniku Windows z uporabo oddaljenega namizja storitve (RDS), prej imenovan terminalskih storitev:
  
- Morate imeti načrt Office 365, ki vključuje Office 365 ProPlus, kot so Office 365 podjetje E3 ali podjetje E5. Office 365 Business in Office 365 Business Premium načrti ne vključujejo Office 365 ProPlus.

- Morate omogočiti [skupno aktivacija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Če želite namestiti Office 365 ProPlus na RDS na portalu Office 365, ** *ki uporablja privzeto nastavitev za namestitev* **, sledite tem korakom:
  
1. Ček kakšen načrt Office 365. [Učenje kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Če je potrebno, stikalo za različne Office 365 načrt. [Učenje kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Če je Office že nameščen na RDS strežnika z uporabo načrti za Office 365, ga odstranite. Na primer, z tekoč v pregled slika na lesu \> Uninstall program. Odstraniti z uporabo [Microsoft podporo in regres pomočnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če uporabljate problematike.

4. Na RDS strežnika, prijavite portalu Office 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Ko namestite Office, ** *ne odpreti ali znamenje v* ** za vse Officeove programe.

6. Na RDS strežnika, omogočiti aktiviranje porazdeliti računalo z urejanjem registra z naslednjim korakom:

1. Z desno miškino tipko gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit**in izberite OK.

2. Izbrati o čas sufler omogočiti registracija urednik narediti spremembe na napravi.

3. V registracija urednik, dodajte vrednost niza za **SharedComputerLicensing** z nastavitvijo 1 pod HKEY_LOCAL_MACHINESOFTWAREMicrosoft\ \Office\ClickToRun\Configuration.

7. V strežniku RDS ** *vpisati kot končnega uporabnika* ** in [Preverite, ali rabi aktivacija omogočen za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Za več podrobnosti o pogoji, navodila za namestitev in navodila glede namestitve po meri z orodjem Office uvajanja, glejte [Uvajanje Office 365 ProPlus z uporabo storitve oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Za odpravljanje napak, povezanih v skupni rabi activation, prosimo, glejte [Odpravljanje težav s skupno aktivacija za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  