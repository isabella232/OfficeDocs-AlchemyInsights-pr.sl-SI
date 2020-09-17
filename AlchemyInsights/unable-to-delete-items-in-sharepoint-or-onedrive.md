---
title: Elementov v SharePointu ali OneDrive ni mogoče izbrisati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806127"
---
# <a name="unable-to-delete-items"></a>Elementov ni mogoče izbrisati

Pravilniki o hranjenju lahko povzročijo to težavo, vendar morate onemogočiti ali izključiti ustrezno zadržanje, ki povzroča to težave. Ko je pravilnik o hranjenju ali zadržanje odstranjen, lahko traja do 24 ur, da začne veljati sprememba. Zagotovite, da v elementu ni nastavljene nastavitve [pravilnika o hranjenju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .

Mesto je morda preseglo omejitev shrambe, povečanje [količinske omejitve mesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) in brisanje elementa.

Zagotovite, da element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.

Na koncu lahko skrbniki uporabljajo [SharePointove vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ki vsebuje knjižnico ukazov PowerShell, ki omogočajo izvajanje zapletenih dejanj upravljanja, kot je na primer Vsiljevanje brisanja trmastih elementov.
- [Odstranjevanje datoteke PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstranjevanje mape PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstranjevanje elementa seznama PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstranjevanje seznama PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstranjevanje polja PNP (stolpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)