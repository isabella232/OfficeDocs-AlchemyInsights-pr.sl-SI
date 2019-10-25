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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682296"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odpravite težave pri dostavi e-pošte za kodo napake 5.7.23

Preverite SPF DNS zapis za vašo domeno na javno voljo SPF ali DNS zapis Checker na spletu.

Preverite, da odhodno sporočilo ni bilo identificirane kot vsiljena pošta s strani Officea 365 in Preusmerjeno prek [bazena za dostavo z visokim tveganjem](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Sporočila v skupini za dostavo z visokim tveganjem ne bodo uspešno preverila SPF-jev, zato jih organizacija ciljne e-pošte ne bo sprejela.

Če težave ne odpravite, se boste morda morali obrniti na skrbnika poštnega gostitelja, na katerega poskušate poslati e-poštno sporočilo. Zapišite si podrobno zunanjo napako, ki je na voljo v sporočilu za odklonovanje.  Podpora za Office 365 morda ne bo mogla dodatno pomagati.