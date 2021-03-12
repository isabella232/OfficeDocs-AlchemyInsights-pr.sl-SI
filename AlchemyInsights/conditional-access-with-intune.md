---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704802"
---
# <a name="conditional-access-with-intune"></a>Pogojni dostop z InTune

Uporaba  **pogojnega dostopa**  s funkcijo InTune zahteva 3 korake:

- Ustvarite  **pravilnik o skladnosti**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), da določite nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za skladno. Na primer, mora imeti naprava PIN vsaj 6 števk, preden se šteje za združljivo.
- Ustvarjanje **pravilnika za pogojni dostop**  , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolnjevati za dostop do teh virov.  Naprava mora biti na [primer](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) združljiva pred dostopom do e-pošte podjetja.
- Zagotovite, da bodo **Pravilniki o skladnosti**  in  **Pravilniki pogojnega dostopa**  usmerjeni na želene skupine uporabnikov. S tem boste morda morali ustvariti določene skupine uporabnikov v storitvi Azure Active Directory.

**Uporabne povezave:**

[Pregled skladnosti naprave](https://docs.microsoft.com/intune/device-compliance-get-started)

[Odpravljanje težav CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Pravilnik za odpravljanje težav](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Za zaščito e-pošte (Exchange Online) iz Accessa z nezdružljivimi napravami je treba upoštevati oba dokumenta:

1. [Zaščita e-poštnega dostopa v napravah s storitvijo EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaščita e-pošte v napravah s sodobnimi strankami za preverjanje pristnosti, kot je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)