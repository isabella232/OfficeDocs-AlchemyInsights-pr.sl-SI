---
title: Sporočila, poslana skupini Microsoft 365, ne prejmejo vsi člani
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: sl-SI
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051517"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Sporočila, poslana skupini Microsoft 365, ne prejmejo vsi člani

Prepričajte se, da so vsi člani skupine naročeni na prejemanje e-poštnih sporočil. Glejte [spremljanje skupine v programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Če želite preveriti stanje sporočila članov, ki so naročeni na skupinske e-pošte, zaženite ta ukaz na [exo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`