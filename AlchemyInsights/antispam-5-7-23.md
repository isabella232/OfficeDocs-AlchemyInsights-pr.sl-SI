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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676513"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23

Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.

Prepričajte se, da Microsoft odhodno sporočilo ni bilo identificiran kot vsiljena pošta in preusmerjen prek [paketa za dostavo z visokim tveganjem](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.

Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo. Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje. Microsoftova podpora morda ne bo mogla dodatno pomagati.
