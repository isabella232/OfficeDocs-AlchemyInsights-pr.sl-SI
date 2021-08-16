---
title: Ni mogoče izbrisati elementov v SharePoint ali OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038533"
---
# <a name="unable-to-delete-items"></a>Elementov ni mogoče izbrisati

- Pravilniki o hranjenju lahko povzročijo, da onemogočite ali izključite ustrezno zadržanje, ki povzroča to težavo. Ko je pravilnik o hranjenju ali zadržanje odstranjeno, lahko traja do 24 ur, preden začne sprememba veljati. Prepričajte se, da za [element ni nastavljen](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pravilnik o hranjenju.

- Spletno mesto je morda preseglo omejitev shrambe, povečalo [količinsko omejitev mesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) in izbrisalo element.

- Prepričajte se, da element [ni rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.

- Skrbniki lahko na koncu [uporabijo vzorce SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) prakse (PnP), ki vsebuje knjižnico ukazov ogrodja PowerShell, s katerimi lahko izvajate zapletena dejanja upravljanja, na primer vsili brisanje neustavnejših elementov.
- [Odstrani datoteko PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrani mapo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrani element seznama PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrani seznam PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstranjevanje polja PNP (stolpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)