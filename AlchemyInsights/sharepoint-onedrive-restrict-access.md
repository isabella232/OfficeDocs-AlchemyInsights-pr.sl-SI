---
title: Omejevanje dostopa v SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093858"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePoint ali OneDrive

Dostop do spletnih storitev lahko omejite na SharePoint Online/OneDrive. Spodaj so opisani ti različni načini omejitev dostopa. 

**Omejitev dovoljenj**

V SharePoint Online in OneDrive za podjetja omejujemo dostop do elementov, kot so mesta, datoteke in mape, tako da dostop do teh skupin/posameznikov odobrimo le osebam, ki bi morale imeti dostop.

- [Prilagajanje dovoljenj za seznam SharePoint ali knjižnico](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagajanje SharePoint mesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Spreminjanje dovoljenj v podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nadzor dostopa iz neu upravljanje naprav](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kot SharePoint ali globalni skrbnik lahko blokirate ali omejite dostop do vsebine SharePoint in OneDrive iz neu upravljanje naprav (naprave, ki niso pridružene hibridnemu programu AD ali skladne s predpisi storitve Intune).

**Omejitev omrežnega mesta**

Kot skrbnik za IT lahko nadzorujete dostop do razpoložljivih SharePoint in OneDrive na podlagi določenih omrežnih mest, ki jim zaupate. To imenujemo tudi pravilnik na osnovi lokacije. Če želite več informacij, glejte [Nadzor dostopa SharePoint spletu in OneDrive podatkov na podlagi omrežnega mesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Omejitev zaklepanja mesta** 

V SharePoint Online lahko zaklenete zbirko mest, tako da nihče nima dostopa. To nastavitev nastavite prek lupine PowerShell [in ukazne lupine SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) z lastnostjo [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Omejevanje uporabnikov pred ustvarjanjem mest ali podmest**

Kot SharePoint skrbnik ali globalni skrbnik lahko uporabnikom omogočite ustvarjanje in skrbništvo njihovih mest SharePoint, določanje vrste spletnih mest, ki jih lahko ustvarijo, in določanje mesta mest. Če želite več informacij, glejte [Upravljanje ustvarjanja spletnih mest v SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)

