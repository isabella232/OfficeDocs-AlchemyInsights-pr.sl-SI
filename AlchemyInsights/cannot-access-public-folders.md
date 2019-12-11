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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959510"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne more vzpostaviti povezave z javnimi mapami

Če dostop do javne mape za nekaj uporabnikov ne deluje, poskusite to:

Povežite se z lupino EXO PowerShell in konfigurirajte DefaultPublicFolderMailbox na težavi uporabniški račun, da se ujemajo z enim na delovnem uporabniškem računu.

Primer:

Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, Efetivepublicfoldermailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<vrednost iz prejšnjega ukaza>

Počakajte vsaj eno uro, da sprememba učinkuje.