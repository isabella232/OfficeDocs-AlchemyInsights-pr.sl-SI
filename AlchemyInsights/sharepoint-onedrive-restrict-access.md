---
title: Omejevanje dostopa v SharePoint ali OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223728"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePoint ali OneDrive

Obstaja veliko načinov za preprečevanje dostopa do storitve SharePoint Online/OneDrive. Te različne metode za omejitev dostopa so opisani spodaj. 

**Dovoljenje omejitve**

V SharePoint Online in OneDrive za poslovanje, smo omejiti dostop do predmetov, kot so spletna mesta, datoteke in mape samo odobri dostop do tistim skupinam/posameznikom, ki bi morali imeti dostop.

- [Prilagodite dovoljenj za SharePointov seznam ali knjižnico](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodite dovoljenja mesta SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Spremenite dovoljenja, podmape](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nadzor dostopa iz neupravljane naprave](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kot SharePoint ali svetovnih admin v Office 365, lahko blokirate ali omejiti dostop do vsebin, SharePoint in OneDrive iz neupravljane naprave (teh hibridnih AD pridružil ali ustrežljiv v Intune).

**Omrežno mesto omejitev**

Kot IT admin, lahko nadzor dostopa do virov SharePoint in OneDrive, na osnovi določenih omrežnih mest, ki jim zaupate. To je znana tudi kot namestitev-osnova politike. Če želite več informacij, si oglejte [pregled postranski v SharePoint Online in OneDrive podatke, ki temeljijo na omrežno mesto](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Omejitve mesta Lock** 

V SharePoint Online imate sposobnost za zaklepanje določitvi mest, tako da nihče ni dostopa. To se nahaja preko PowerShell in [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) uporabite lastnost - LockState [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

**Določim, da ustvarjanje mest ali podmesta**

Kot SharePoint admin ali Office 365 svetovnih admin, lahko pustite vaš uporabnik ustvariti in upravljati svoje lastne SharePointovih mest, ugotoviti, kakšne strani, ki jih lahko ustvarite, določite lokacijo mesta. Če želite več informacij, si oglejte [Ustvarjanje upravljanje mesta v SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

