---
title: Uvajanje ekip kot samostojne ali z novimi ali obstoječimi Officeovimi namestitvami
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806775"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Uvajanje ekip kot samostojne ali z novimi ali obstoječimi Officeovimi namestitvami

Microsoft Teams je zdaj vključen kot del ***novih namestitev*** programov Microsoft 365 za podjetja, Microsoft 365 apps za podjetja in Office za Mac. Če želite več informacij, glejte [Kdaj bo Microsoft Teams začel uporabljati nove namestitve Officea?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Poleg tega se bodo v napravah s sistemom Windows, ko posodobite obstoječo namestitev na najnovejšo različico, začele s 1906 različicami v trenutnem kanalu, bo ekipam ***dodana v obstoječe namestitve*** aplikacij Microsoft 365 za podjetja (in Microsoft 365 apps za podjetja). Če želite več informacij, glejte [Kaj je z obstoječimi namestitvami Officea?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Če ne želite počakati na ta razpored uvajanja, lahko za uporabnike uvedete skupine kot samostojne, tako da [upoštevate ta navodila](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ali pa lahko uporabniki sami namestijo ekipe  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Če vaša organizacija ni pripravljena na uvedbo ekip, imamo navodila, s katerimi lahko ***izključite ekipe*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ali [obstoječih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) namestitev Officea. Če želite, da bodo ekipe nameščene, vendar ne želite, da se ekipe samodejno zaženejo za uporabnika po namestitvi, si oglejte preprečite, da bi se [Microsoft Teams po namestitvi samodejno](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)zagnal.

Če želite ***odstraniti ekipe*** iz naprave, v kateri se izvaja Windows, glejte [odstranitev aplikacije Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Če želite Microsoft Teams počistiti iz več ciljnih strojev ali uporabnikov, si oglejte [uvajanje storitve Microsoft Teams Clean Up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Če uporabljate računalnike v skupni rabi, oddaljene namizne storitve (RDS) ali navidezne namizne infrastrukture (VDI), si oglejte [računalnike v skupni rabi in okolja VDI z aplikacijo Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Če uporabljate Office za Mac, glejte [naprave Microsoft Teams v računalniku Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Ko je ekipa nameščena, se [samodejno posodobi](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približno vsaka dva tedna z novimi funkcijami in posodobitvami kakovosti. 