---
title: Uporaba pogojnega dostopa s funkcijo InTune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749263"
---
# <a name="using-conditional-access-with-intune"></a>Uporaba pogojnega dostopa s funkcijo InTune

Uporaba pogojnega dostopa s funkcijo InTune zahteva 3 korake:

- [Ustvarite pravilnik o skladnosti, da določite nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za skladno. Na primer, mora imeti naprava PIN vsaj 6 števk, preden se šteje za združljivo.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Ustvarjanje pravilnika za pogojni dostop, ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolnjevati za dostop do teh virov. Naprava mora biti na primer združljiva pred dostopom do e-pošte podjetja.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zagotovite, da bodo pravilniki o skladnosti in pravilniki pogojnega dostopa usmerjeni na želene skupine uporabnikov. S tem boste morda morali ustvariti določene skupine uporabnikov v storitvi Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Več informacij ...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
