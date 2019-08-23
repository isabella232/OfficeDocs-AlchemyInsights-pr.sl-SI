---
title: Ni mogoče izbrisati elemente v SharePoint ali OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558669"
---
# <a name="unable-to-delete-items"></a>Ni mogoče izbrisati elemente

Ob vprašanjih izbrisom SharePoint?

- Vedno preverite, ali imate [ustrezna dovoljenja](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) za brisanje elementa ali so [skrbnike](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) poskus, odstranite element.

- Zagotoviti, da je ne setup [zadrževanja](https://docs.microsoft.com/office365/securitycompliance/retention-policies) na element.

- Zagotoviti element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.

- Končno, lahko skrbniki [SharePoint vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ki vsebuje knjižnico PowerShell ukaze, ki omogočajo izvajanje zapletenih upravljanjem, kot sila izbrisom trmast.
- [Odstranite datoteko PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstranite PNP mapo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstranite element seznama PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstranite PNP seznam](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstranite PNP polju (stolpcu)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)