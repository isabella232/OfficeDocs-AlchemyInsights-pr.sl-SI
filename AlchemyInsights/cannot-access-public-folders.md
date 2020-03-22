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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891765"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne more vzpostaviti povezave z javnimi mapami

Če dostop do javne mape za nekatere uporabnike ne deluje, poskusite to:

Povežite se z lupino EXO in konfigurirajte parameter DefaultPublicFolderMailbox na uporabnikovem uporabniškem računu, da se ujema s parametrom v delovnem uporabniškem računu.

Primer:

Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, Efetivepublicfoldermailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<vrednost iz prejšnjega ukaza>

Počakajte vsaj eno uro, da sprememba učinkuje.

Če težava ostane, upoštevajte [ta postopek](https://aka.ms/pfcte) , če želite odpraviti težave z dostopom do javnih map z Outlookom.