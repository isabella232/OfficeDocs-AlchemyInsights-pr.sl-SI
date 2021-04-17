---
title: Dostop do javnih map ni na voljo
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819528"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne more povezati z javnimi mapami

Če dostop do javnih map ne deluje za nekatere uporabnike, poskusite to:

Vzpostavite povezavo z exo PowerShell in konfigurirajte parameter DefaultPublicFolderMailbox za težaveni uporabniški račun, da se bo ujemal s parametrom v delovnem uporabniškem računu.

Primer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox TežavaUporabnik -DefaultPublicFolderMailbox \<value from previous command>

Počakajte vsaj eno uro, da sprememba začne veljati.

Če težave ne odpravite, upoštevajte ta [postopek](https://aka.ms/pfcte) in odpravite težave z dostopom do javnih map z Outlookom.
 
**Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map v Outlooku:**

1.  Uporabite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ali $false  
      
    $true: Omogočanje dostopa uporabnikom do javnih map v Outlooku  
      
    $false: Preprečite uporabnikom dostop do javnih map v Outlooku. To je privzeta vrednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Opomba** S tem postopkom lahko nadzorujete povezave le z namiznim programom Outlook za Windows. Uporabnik lahko še naprej dostopa do javnih map s programom OWA ali Outlook for Mac.
 
Če želite več informacij, [glejte Napove najavljena podpora za nadzorovane povezave do javnih map v Outlooku.](https://aka.ms/controlpf)