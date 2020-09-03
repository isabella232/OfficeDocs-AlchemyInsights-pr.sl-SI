---
title: Dostop do javnih map ni mogoč
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341419"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne more povezati z javnimi mapami

Če dostop do javne mape ne deluje za nekatere uporabnike, poskusite to:

Povežite se s EKSO PowerShell in konfigurirajte parameter DefaultPublicFolderMailbox v uporabniškem računu težave, da se ujema s parametrom v delujočem uporabniškem računu.

Primer

Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Nastavitev nabiralnika ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Počakajte vsaj eno uro, da sprememba začne veljati.

Če težava ostane, upoštevajte [ta postopek](https://aka.ms/pfcte) , da odpravite težave z dostopom do javnih map z Outlookom.
 
**Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map z Outlookom**:

1.  Uporabite ukaz» Set-CASMailbox <mailboxname> -PublicFolderClientAccess «$TRUE ali $FALSE  
      
    $true: Omogočanje uporabnikom dostop do javnih map v Outlooku  
      
    $false: preprečite uporabniku dostop do javnih map v Outlooku. To je privzeta vrednost.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Opomba** S tem postopkom lahko nadzorujete povezave le s programom Outlook Desktop za odjemalce sistema Windows. Uporabnik lahko še naprej dostopa do javnih map s programom OWA ali Outlook za Mac.
 
Če želite več informacij, glejte [objava podpore za nadzorovane povezave z javnimi mapami v Outlooku](https://aka.ms/controlpf).