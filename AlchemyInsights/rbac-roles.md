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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583953"
---
# <a name="rbac-rules"></a>Pravila RBAC

Če se prikaže napaka» dovoljenje «: 

- **Odjemalec z ID-jem predmeta nima dovoljenja za izvajanje dejanj nad obsegom (koda: AuthorizationFailed)**: ko poskušate ustvariti vir, preverite, ali ste trenutno vpisani z uporabnikom, ki je dodeljen vlogi, ki ima dovoljenje za pisanje za vir v izbranem obsegu. Če želite na primer upravljati virtualne stroje v skupini virov, morate imeti vlogo [navideznega stroja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) v skupini virov (ali nadrejenem obsegu). Če želite seznam dovoljenj za vsako vgrajeno vlogo, glejte [vgrajene vloge za vire Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Nimate **dovoljenja za ustvarjanje zahteve za podporo**: ko poskušate ustvariti ali posodobiti vstopnico za podporo, se prepričajte, da ste trenutno vpisani z uporabnikom, ki je dodeljen vlogi, ki ima Microsoftovo dovoljenje za podporo/supportTickets/pisanje, kot je na primer [Podpora za zahtevo](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Ne morete ustvariti več dodelitev vlog (koda: RoleAssignmentLimitExceeded)**: ko poskušate dodeliti vlogo, poskusite zmanjšati število dodelitev vlog tako, da dodelite vloge skupinam. Azure podpira do **2000** dodelitev vlog na naročnino.

Če želite več informacij o vlogah Azure RBAC, glejte vloge v storitvi [AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
