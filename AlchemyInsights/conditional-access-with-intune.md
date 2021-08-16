---
title: Pogojni dostop s funkcijo Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069728"
---
# <a name="conditional-access-with-intune"></a>Pogojni dostop s funkcijo Intune

Za  **uporabo pogojnega dostopa**  s storitvijo Intune so potrebni 3 koraki:

- Ustvarite pravilnik **za skladnost** s predpisi [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), da določite nastavitve, ki morajo biti v napravi izpolnjene, preden je naprava skladna. Naprava na primer velja za skladno le, če ima vsaj 6 števk PIN.
- Ustvarite pravilnik **pogojnega dostopa,**  ki določa, kateri viri so zaščiteni in kateri pogoji morajo biti izpolnjeni, če želite dostopati do teh virov.  [Naprava na primer mora](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  biti skladna, preden je z dostopom do poslovne e-pošte dostopna.
- Zagotovite, **da sta pravilnik o**  skladnosti s  **predpisi**  in pravilnik pogojnega dostopa namenjena želenim skupinam uporabnikov. Zaradi tega boste morda morali ustvariti posebne skupine uporabnikov v Azure Active Directory.

**Koristne povezave:**

[Pregled skladnosti naprave s predpisi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Odpravljanje težav s ca-jem](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik za odpravljanje težav](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Če želite e-pošto (Exchange spletu) pred dostopom prek naprav, ki niso v skladu s spletom, morate upoštevati oba dokumenta:

1. [Zaščitite dostop do e-pošte v napravah s storitvijo EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaščitite dostop do e-pošte v napravah s sodobnimi odjemalci za preverjanje pristnosti, kot Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)