---
title: Uvajanje ekip kot samostojnih ali z novimi ali obstoječimi Officeovimi namestitvami
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617911"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Uvajanje ekip kot samostojnih ali z novimi ali obstoječimi Officeovimi namestitvami

Microsoft Teams je zdaj vključen kot del ***novih naprav*** Microsoft 365 apps za podjetja, Microsoft 365 Apps for Business in Office for Mac. Če želite več informacij, glejte [Kdaj bo Microsoft Teams začel biti vključen v nove namestitve Officea?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Poleg tega, začenši z različico 1906 v trenutnem kanalu, bodo ekipe ***dodane obstoječim napravam*** Microsoft 365 apps za podjetja (in Microsoft 365 Apps for Business) v napravah z operacijskim sistemom Windows, ko posodobite obstoječo namestitev na najnovejšo različico. Če želite več informacij, preberite [kaj o obstoječih namestitvah Officea?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Če ne želite čakati na ta urnik uvajanja, lahko skupine nastavite kot samostojne za uporabnike tako, da [upoštevate ta navodila](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ali pa lahko uporabniki namestijo ekipe sami od sebe  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Če organizacija ni pripravljena za uvajanje ekip, imamo korake, ki jih lahko vzamete za ***izključitev ekip*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ali [obstoječih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) namestitvah Officea. Če želite, da se ekipe namestijo, vendar ne želite, da se ekipe samodejno zažene za uporabnika po namestitvi, glejte [Preprečevanje samodejnega zagona programa Microsoft Teams po namestitvi](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Če želite ***odstraniti ekipe*** iz naprave, v kateri se izvaja sistem Windows, glejte [odstranjevanje Microsoftovih ekip](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Če želite počistiti Microsoft Teams iz več ciljnih naprav ali uporabnikov, glejte [čiščenje programa Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Če uporabljate računalnike v skupni rabi, storitve oddaljenega namizja (RDS) ali infrastrukturo navideznega namizja (VDI), si oglejte [okolja v skupni rabi in VDI z Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Če uporabljate Office for Mac, glejte [naprave Microsoft Teams v računalniku Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Ko je program Teams nameščen, se [samodejno posodablja](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približno vsaka dva tedna z novimi funkcijami in posodobitvami kakovosti. 