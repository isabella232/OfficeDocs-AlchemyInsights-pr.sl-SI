---
title: Nadzor dostopa do javnih map s Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032574"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Nadzor dostopa do javnih map s Outlook

Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map Outlook:

1. Uporaba `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Omogočanje dostopa uporabnikom do javnih map v Outlook  
$false: Preprečite uporabnikom dostop do javnih map v Outlook. To je privzeta vrednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Opomba: S tem postopkom lahko nadzorujete le povezave z Outlook za Windows odjemalce. Uporabniki lahko še naprej dostopajo do javnih map s programom OWA ali Outlook za Mac.

Če želite več informacij, glejte [Nadzorovane povezave z javnimi mapami Outlook](https://aka.ms/controlpf) mestu.
