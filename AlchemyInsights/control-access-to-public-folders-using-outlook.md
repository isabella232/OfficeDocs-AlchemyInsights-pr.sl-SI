---
title: Nadzor dostopa do javnih map z Outlookom
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816756"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Nadzor dostopa do javnih map z Outlookom

Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map v Outlooku:

1. Uporaba `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Omogočanje dostopa uporabnikom do javnih map v Outlooku  
$false: Preprečite uporabnikom dostop do javnih map v Outlooku. To je privzeta vrednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Opomba: S tem postopkom lahko nadzorujete le povezave z namiznimi odjemalci za Outlook za Windows. Uporabniki lahko še naprej dostopajo do javnih map s programom OWA ali Outlook for Mac.

Če želite več informacij, glejte [Nadzorovane povezave z javnimi mapami v Outlooku.](https://aka.ms/controlpf)
