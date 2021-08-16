---
title: Uvajanje predmeta pravilnika skupine
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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067856"
---
# <a name="gpo-deployment"></a>Uvajanje predmeta pravilnika skupine

Nastavitve za uporabniške in računalniške predmete v Azure Active Directory Domain Services (Azure AD DS) se pogosto upravljajo s predmeti pravilnika skupin. Azure AD DS vključuje vgrajene gpote za uporabnike AADDC in vsebnike računalnikov AADDC. Te vgrajene pravilnike skupin lahko prilagodite tako, da za okolje konfigurirate pravilnik skupine po potrebi. Člani skupine skrbnikov imenika Azure AD DC imajo skrbniške pravice pravilnika skupine v domeni Azure AD DS, lahko pa ustvarijo tudi gpote po meri in organizacijske enote (OU). Če želite več informacij o tem, kaj je pravilnik skupine in kako deluje, glejte [Pregled pravilnika skupine.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

V hibridnem okolju se pravilniki skupin, konfigurirani v okolju AD DS na mestu uporabe, ne sinhronizirajo s storitvijo Azure AD DS. Če želite določiti nastavitve konfiguracije za uporabnike ali računalnike v storitvi Azure AD DS, uredite enega od privzetih pravilnikov skupin po meri ali ustvarite predmet pravilnika skupin po meri.

V tem [članku je](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) prikazano, kako namestite orodja za upravljanje pravilnika skupin, kako tona uredi vgrajene predmete pravilnikov skupin in kako ustvarite pravilnike skupin po meri.
