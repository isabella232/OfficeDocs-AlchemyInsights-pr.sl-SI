---
title: Uporaba spletnega mesta Wix s Office 365 kupljenih ali upravljanih domen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980193"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Uporaba spletnega mesta Wix s Office 365 kupljenih ali upravljanih domen

- [Posodabljanje zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Članek Wix »Connecting a Domain to Wix Using the Pointing Method« (Povezovanje domene z omrežjem Wix s kazalno metodo) priporočamo, da namesto spreminjanja imenskih strežnikov uporabite kazalo (dodajanje zapisov DNS na zgornjo povezavo) namesto da spremenite imenski strežnik Office 365
- Če se še vedno odločite za spreminjanje imenskih strežnikov v Wix, boste morali ustvariti zapise  [DNS na spletnem mestu Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Če ste domeno kupili pri Microsoftu, imenskih strežnikov ni mogoče spremeniti. Če morate spremeniti strežnike z imeni, ki jih je kupil Microsoft, morate po 60 dneh prenesti k  [drugemu ponudniku gostovanja.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)