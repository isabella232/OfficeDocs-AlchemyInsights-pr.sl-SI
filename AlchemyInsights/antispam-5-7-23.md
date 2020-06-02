---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506459"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23

Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.

Prepričajte se, da Microsoft odhodno sporočilo ni bilo identificiran kot vsiljena pošta in preusmerjen prek [paketa za dostavo z visokim tveganjem](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.

Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo. Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje. Microsoftova podpora morda ne bo mogla dodatno pomagati.
