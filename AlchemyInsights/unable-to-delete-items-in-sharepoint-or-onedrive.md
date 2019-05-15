---
title: Ni mogoče izbrisati elemente v SharePoint ali OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057776"
---
# <a name="unable-to-delete-items"></a>Ni mogoče izbrisati elemente

Ob vprašanjih, brisanje elementov?

- Vedno preverite, ali imate [ustrezna dovoljenja](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) za brisanje elementa ali so [skrbnike](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) poskus, odstranite element.

- Zagotoviti, da je ne setup [zadrževanja](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) na element.

- Zagotoviti element ni [rezerviran](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.

- Končno, lahko skrbniki [SharePoint vzorce in prakse](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ki vsebuje knjižnico PowerShell ukaze, ki omogočajo izvajanje zapletenih upravljanjem, kot sila izbrisom trmast. 
- [Odstranite datoteko PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstranite PNP mapo](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstranite element seznama PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstranite PNP seznam](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstranite PNP polju (stolpcu)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)