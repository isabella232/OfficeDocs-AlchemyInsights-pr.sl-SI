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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813704"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Napaka »Pri sprejemanju žetona za dostop je prišlo do napake«

Ta napaka je običajno opazovana, ko poteče žeton za preverjanje pristnosti. Če osvežite stran, osvežite žeton. Vendar pa lahko ta težava še vedno obstaja, če obstajajo pravilniki pogojnega dostopa, uporabljeni za račun, ki se uporablja za namizno analitiko na tabli. Na portalu Azure Portal si lahko ogledate dnevnike vpisa v Azure AD in si ogledate, ali je prišlo do napak pri vpisu za račun, ki se uporablja za vpis v Namizno analitiko.

Če želite več informacij o pogojnem dostopu, [obiščite spletno mesto Načrtovanje uvajanja pogojnega dostopa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)