---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931452"
---
# <a name="conditional-access-with-intune"></a>Pogojni dostop z InTune

Uporaba **pogojnega dostopa** z InTune zahteva 3 korake:

- Ustvarite **pravilnik o skladnosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), da določite nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za združljivo. Naprava mora imeti na primer PIN vsaj 6 števk, preden se šteje za skladno.
- Ustvarite **pravilnik pogojnega dostopa** , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolniti za dostop do teh virov.  Naprava mora biti na [primer](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) skladna pred dostopom do e-pošte podjetja.
- Zagotovite, da so pravilniki o **skladnosti** in **Pravilniki o pogojnem dostopu** usmerjeni na želene skupine uporabnikov. To lahko zahteva ustvarjanje določenih skupin uporabnikov v storitvi Azure Active Directory.

**Koristne povezave:**

[Pregled skladnosti naprave](https://docs.microsoft.com/intune/device-compliance-get-started)

[Odpravljanje težav s certifikatnega urada](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik o odpravljanju težav](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Za zaščito e-pošte (Exchange Online) od dostopa, ki ga nezdružljive naprave, je treba upoštevati oba dokumenta:

1. [Zaščitite e-poštni dostop iz naprav, ki uporabljajo EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaščitite e-poštni dostop iz naprav s sodobnimi odjemalci za preverjanje pristnosti, kot je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)