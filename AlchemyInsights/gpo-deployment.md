---
title: Uvajanje pravilnika skupine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428052"
---
# <a name="gpo-deployment"></a>Uvajanje pravilnika skupine

Nastavitve za predmete uporabnika in računalnike v domenskih storitvah Azure Active Directory (Azure AD DS) pogosto upravljajo s predmeti pravilnika skupine (GPO-ji). Azure AD DS vključuje vgrajene GPO-je za uporabnike AADDC in AADDC računalnike. Te vgrajene GPO-je lahko prilagodite tako, da konfigurirate pravilnik skupine, kot je potrebno za vaše okolje. Člani skupine» Skrbniki v storitvi Azure AD DC «imajo skrbniške pravice pravilnika skupine v domeni Azure AD DS, lahko pa tudi ustvarijo GPO in organizacijske enote po meri (organizacijske). Če želite več informacij o tem, kaj je pravilnik skupine in kako deluje, glejte [pregled pravilnika skupine](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

V hibridnem okolju se pravilniki skupine, konfigurirani v okolju na mestu uporabe AD DS, ne sinhronizirajo s storitvijo Azure AD DS. Če želite določiti nastavitve konfiguracije za uporabnike ali računalnike v storitvi Azure AD DS, uredite enega od privzetih GPO-jev ali ustvarite GPO po meri.

V tem članku je [upravljanje pravilnika skupine](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) prikazano, kako namestite orodja za upravljanje pravilnika skupine, kako lahko tone uredite vgrajene GPO-je in kako ustvarite GPO-je po meri.
