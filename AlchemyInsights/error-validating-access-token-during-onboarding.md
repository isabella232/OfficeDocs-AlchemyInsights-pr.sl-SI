---
title: Med preverjanjem veljavnosti žetona za dostop med storitvijo Desktop Analytics na tabli je prišlo do napake
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946631"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Napaka »Pri sprejemanju žetona za dostop je prišlo do napake«

Ta napaka je običajno opazovana, ko poteče žeton za preverjanje pristnosti. Če osvežite stran, osvežite žeton. Vendar pa lahko ta težava še vedno obstaja, če obstajajo pravilniki pogojnega dostopa, uporabljeni za račun, ki se uporablja za namizno analitiko na tabli. Na portalu Azure Portal si lahko ogledate dnevnike vpisa v Azure AD in si ogledate, ali je prišlo do napak pri vpisu za račun, ki se uporablja za vpis v Namizno analitiko.

Če želite več informacij o pogojnem dostopu, [obiščite spletno mesto Načrtovanje uvajanja pogojnega dostopa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)