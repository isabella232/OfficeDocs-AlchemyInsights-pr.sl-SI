---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717341"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odpravljanje težav z dostavo e-pošte za kodo napake 5.7.23

Preverite zapis SPF DNS za svojo domeno na javno razpoložljivem pregledovalniku SPF ali DNS v spletu.

Preverite, ali je Microsoft in preusmerjeni prek [paketa z visokim tveganjem](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages), ki ga je navedla neželena sporočila. Sporočila v skupini z visokim tveganjem ne bodo posredovala preverjanja SPF, zato je ne bo sprejela ciljna e-poštna organizacija.

Če težave ne morete odpraviti, se boste morda morali obrniti na skrbnika poštnega gostitelja, v katerega želite poslati e-pošto. Seznanite se s podrobno zunanjo napako, ki je na voljo v sporočilu Bounce. Microsoftova podpora morda ne bo mogla več pomagati.
