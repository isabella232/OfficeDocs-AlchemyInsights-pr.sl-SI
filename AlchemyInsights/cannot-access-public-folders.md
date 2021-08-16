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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996646"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook povezave z javnimi mapami ni mogoče vzpostaviti

Če dostop do javnih map ne deluje za nekatere uporabnike, poskusite to:

Povezovalnik exo PowerShell in konfigurirajte parameter DefaultPublicFolderMailbox za uporabniški račun težave tako, da se ujema s parametrom v delovnem uporabniškem računu.

Primer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox TežavaUporabnik -DefaultPublicFolderMailbox \<value from previous command>

Počakajte vsaj eno uro, da sprememba začne veljati.

Če težave ne odpravite, upoštevajte ta [postopek](https://aka.ms/pfcte) in odpravite težave z dostopom do javnih map Outlook.
 
**Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map Outlook:**

1.  Uporabite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ali $false  
      
    $true: Omogočanje dostopa uporabnikom do javnih map v Outlook  
      
    $false: Preprečite uporabnikom dostop do javnih map v Outlook. To je privzeta vrednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Opomba** S tem postopkom lahko nadzorujete povezave le z Outlook za Windows odjemalce. Uporabnik lahko še naprej dostopa do javnih map s programom OWA ali Outlook za Mac.
 
Če želite več informacij, [glejte Napove najavljena podpora za nadzorovane povezave z javnimi mapami v Outlook.](https://aka.ms/controlpf)