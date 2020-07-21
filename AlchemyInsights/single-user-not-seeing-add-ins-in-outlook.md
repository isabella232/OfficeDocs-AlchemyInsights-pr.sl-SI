---
title: En uporabnik ne vidi dodatkov v programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198220"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>En uporabnik ne vidi dodatkov v programu Outlook

Uporabnik je morda del vloge, ki nima pravilnega parametra AppsForOfficeEnabled. Zaženite ta ukaz» cmdlet «, če želite izvedeti, ali je pravilna vloga povezana z uporabnikom:

Get-Managementroleodstop-RoleAssignee user@domain.com-delegiranje $false | Format-table-Auto vlogo, RoleAssigneeName, RoleAssigneeType

Če želite več informacij, glejte [določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
