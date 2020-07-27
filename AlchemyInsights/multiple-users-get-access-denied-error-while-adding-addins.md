---
title: Več uporabnikov dobi napako »Dostop zavrnjeno« med dodajanjem dodatkov v programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424175"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Več uporabnikov dobi napako »Dostop zavrnjeno« med dodajanjem dodatkov v programu Outlook

Določite lahko, kateri skrbniki v organizaciji imajo dovoljenja za namestitev in upravljanje dodatkov za Outlook. Določite lahko tudi, kateri uporabniki v vaši organizaciji imajo dovoljenje za namestitev in upravljanje dodatkov za lastno uporabo.

Če želite podrobnosti, [glejte Določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Če želite preveriti, ali ste uporabniku uspešno dodelili dovoljenja, <Role Name> zamenjajte z imenom vloge, ki jo želite preveriti, in zaženite ta ukaz v lupini PowerShell za Exchange Online:

Get-ManagementRoleAssignment -Vloga " <Role Name> " -GetEffectiveUsers

V tem primeru je prikazano, kako preverite, komu ste dodelili dovoljenja za namestitev dodatkov iz Trgovine Office za organizacijo.

Powershell

-Vloga "Org Marketplace Apps" -GetEffectiveUsers

V rezultatih, Get-ManagementRoleAssignment, preglejte vnose v stolpcu Učinkovite uporabnike.

Za podrobne informacije o sintaksi in parametrih [glejte Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 