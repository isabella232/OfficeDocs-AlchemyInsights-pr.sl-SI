---
title: Sporočila, poslana skupini v storitvi Microsoft 365, niso prejeli vsi člani
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 39a4f8115a4742947b3e6394396be5ce3b01e772
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430699"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Sporočila, poslana skupini v storitvi Microsoft 365, niso prejeli vsi člani

Preverite, ali so vsi člani skupine naročeni na prejemanje e-poštnih sporočil. Glejte [Spremljanje skupine v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Če želite preveriti stanje sporočila članov, ki so naročeni na e-poštna sporočila skupine, zaženite ta ukaz [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

S tem ukazom EXO PowerShell konfigurirajte vse člane skupine tako, da prejemajo e-poštna sporočila, poslana skupini v storitvi Microsoft 365, v svojo mapo »Prejeto«:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`