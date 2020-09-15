---
title: Navodila za skrivanje/Razkrij skupino s seznama naslovov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663025"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrij skupino Microsoft 365 na seznamu naslovov (GAL)

Če želite skriti skupino Microsoft 365 s seznamov naslovov (GAL) Exchangeevih odjemalcev (kot je Outlook ali OWA), uporabite ta ukaz v lupini EKSO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Če želite skriti skupino Microsoft 365, ki je vidna v Exchangeevem odjemalcu, uporabite ta ukaz v lupini EKSO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

