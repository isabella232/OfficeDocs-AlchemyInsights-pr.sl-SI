---
title: Uporaba pogojnega dostopa s storitvijo Intune
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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005790"
---
# <a name="using-conditional-access-with-intune"></a>Uporaba pogojnega dostopa s storitvijo Intune

Za uporabo pogojnega dostopa s storitvijo Intune so potrebni 3 koraki:

- [Ustvarite pravilnik o skladnosti s predpisi za določanje nastavitev, ki morajo biti v napravi, preden je naprava skladna. Naprava na primer velja za skladno le, če ima vsaj 6 števk PIN.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Ustvarite pravilnik pogojnega dostopa, ki določa, kateri viri so zaščiteni in kateri pogoji morajo biti izpolnjeni, če želite dostopati do teh virov. Naprava na primer mora biti skladna, preden je z dostopom do poslovne e-pošte dostopna.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zagotovite, da sta pravilnik o skladnosti s predpisi in pravilnik pogojnega dostopa namenjena želenim skupinam uporabnikov. Zaradi tega boste morda morali ustvariti posebne skupine uporabnikov v Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Več informacij ...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
