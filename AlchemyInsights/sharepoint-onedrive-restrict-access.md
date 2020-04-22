---
title: Omejevanje dostopa v SharePointu ali storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692781"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePointu ali storitvi OneDrive

Dostop do storitev SharePoint online/OneDrive lahko omejite na več načinov. Te različne metode omejevanja dostopa so opisane spodaj. 

**Omejitev dovoljenja**

V SharePoint online in OneDrive za podjetja omejimo dostop do elementov, kot so mesta, datoteke in mape, tako da dovoljujemo dostop le tistim skupinam/posameznikom, ki bi morali imeti dostop.

- [Prilagajanje dovoljenj za SharePointov seznam ali knjižnico](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagajanje dovoljenj za SharePointovo mesto](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Spreminjanje dovoljenj v podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nadzor dostopa iz neupravljanih naprav](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kot SharePointov ali globalni skrbnik lahko blokirate ali omejite dostop do vsebine SharePointa in storitve OneDrive iz neupravljanih naprav (tisti, ki niso združeni ali združljivi z AD v InTune).

**Omejitev omrežne lokacije**

Kot skrbnik IT-ja lahko nadzirate dostop do virov SharePoint in OneDrive, ki temeljijo na definiranih omrežnih lokacijah, ki jim zaupate. To je znano tudi kot pravilnik, ki temelji na lokaciji. Če želite več informacij, glejte [nadzor dostopa do podatkov SharePoint online in storitve OneDrive na podlagi omrežnega mesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Omejitev zaklepanja spletnega mesta** 

V spletnem mestu SharePoint online lahko zaklenete zbirko mest, tako da nima dostopa nihče. To je nastavljeno prek lupine PowerShell in [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) z lastnini [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Omejevanje uporabnikov z ustvarjanjem spletnih mest ali podmest**

Kot skrbnik za SharePoint ali globalni skrbnik lahko uporabnikom omogočite ustvarjanje in upravljanje svojih SharePointovih mest, določanje, katere vrste mest lahko ustvarijo, in določite lokacijo mest. Če želite več informacij, glejte [upravljanje ustvarjanja mest v SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

