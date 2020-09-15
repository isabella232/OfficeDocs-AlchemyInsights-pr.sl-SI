---
title: Omejevanje dostopa v SharePointu ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700471"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePointu ali OneDrive

Dostop do storitev SharePoint online/OneDrive lahko omejite na več načinov. Te različne metode omejevanja dostopa so opisane spodaj. 

**Omejitev dovoljenj**

V storitvi SharePoint online in OneDrive za podjetja omejimo dostop do elementov, kot so mesta, datoteke in mape, in sicer tako, da dodeli le dostop do tistih skupin/posameznikov, ki bi morali imeti dostop.

- [Prilagajanje dovoljenj za SharePointov seznam ali knjižnico](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagajanje dovoljenj za SharePointovo mesto](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Spreminjanje dovoljenj v podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nadzor dostopa v neupravljanih napravah](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kot SharePoint ali globalni skrbnik lahko blokirate ali omejite dostop do SharePointovih in OneDrive vsebine iz neupravljanih naprav (tistih, ki niso povezani s hibridnim OGLASom ali pa so združljivi z InTune).

**Omejitev omrežnega mesta**

Kot skrbnik za IT lahko nadzorujete dostop do SharePointovih in OneDrive virov na podlagi določenih omrežnih mest, ki jim zaupate. To je znana tudi kot pravilnik, ki temelji na lokaciji. Če želite več informacij, glejte [nadzor dostopa do podatkov v storitvi SharePoint online in OneDrive, ki temeljijo na omrežnem mestu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Omejitev zaklepanja mesta** 

V storitvi SharePoint online lahko zaklenete zbirko mest, tako da nihče nima dostopa. To je nastavljeno prek lupine PowerShell in storitve [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) z lastnostjo [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Omejevanje uporabnikov pred ustvarjanjem mest ali podmest**

Kot skrbnik za SharePoint ali globalni skrbnik lahko uporabnikom omogočite, da ustvarijo in upravljajo svoja SharePointova mesta, določajo, katere vrste mest, ki jih lahko ustvarijo, in določijo mesto mesta. Če želite več informacij, glejte [upravljanje ustvarjanja mesta v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

