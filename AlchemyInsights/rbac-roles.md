---
title: 'Vloge RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923147"
---
# <a name="rbac-rules"></a>Pravila za RBAC

Če se prikaže napaka dovoljenja: 

- Odjemalec z ID-jem predmeta nima pooblastila za izvajanje dejanja prek obsega **(koda: AuthorizationFailed):** ko poskušate ustvariti vir, preverite, ali ste trenutno vpisani z uporabnikom, ki ima dodeljeno vlogo, ki ima dovoljenje za pisanje za vir v izbranem obsegu. Če želite na primer upravljati navidezne računalnike v skupini virov, morate imeti vlogo navideznega strojnega sodelavka v skupini virov (ali nadrejenem obsegu). [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) Seznam dovoljenj za vsako vgrajeno vlogo najdete v razdelku Vgrajene [vloge za vire Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Nimate **dovoljenja** za ustvarjanje zahteve za podporo: ko skušate ustvariti ali posodobiti vstopnico za podporo, preverite, ali ste trenutno vpisani z uporabnikom, ki ima dodeljeno vlogo Microsoft.Support/supportTickets/write, na primer [Sodelavec](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)zahteve za podporo.
- Ni več mogoče ustvariti nobene dodelitve vloge **(koda: RoleAssignmentLimitExceeded):** ko poskušate dodeliti vlogo, poskusite zmanjšati število dodelitev vlog tako, da dodelite vloge skupinam. Azure podpira do **2000 dodelitev** vlog na naročnino.

Če želite več podrobnosti o vlogah za Azure RBAC, glejte [Vloge za Azure RBAC.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
