---
title: Elementov v SharePointu ali storitvi OneDrive ni mogoče izbrisati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571287"
---
# <a name="unable-to-delete-items"></a>Elementov ni mogoče izbrisati

Pravilniki o hranjenju lahko povzročijo to, zato morate onemogočiti ali izključiti ustrezno zadržanje, ki povzroča to težavo. Ko je pravilnik o hranjenju ali zadržanje odstranjen, lahko traja do 24 ur, da sprememba učinkuje. Zagotovite, da na elementu ni nastavitve [pravilnika o hranjenju](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

Mesto je morda preseglo omejitev shranjevanja, povečalo [kvoto mesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) in zbrisal element.

Zagotovite, da element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugemu uporabniku.

Nazadnje skrbniki lahko uporabljajo [SharePointove vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ki vsebujejo knjižnico ukazov PowerShell, ki vam omogočajo izvajanje zapletenih dejanj upravljanja, kot je vsiliti brisanje trdovratnih elementov.
- [Odstrani datoteko PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrani mapo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrani element seznama PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrani seznam PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrani PNP polje (stolpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)