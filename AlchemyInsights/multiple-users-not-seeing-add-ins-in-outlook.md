---
title: Več uporabnikov, ki ne vidijo dodatkov v programu Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198242"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Več uporabnikov, ki ne vidijo dodatkov v programu Outlook

Če preskusite dodatke Outlook in nobeden ne prikaže, kot prvi korak za odpravljanje težav, uporabite cmdlet **Get-OrganizationConfig** PowerShell za poizvedbo _Appsforofficeenabled_ parameter. Če poizvedba vrne vrednost **FALSE**, nastavite ta parameter na **True** z ukazom» cmdlet « **Set-OrganizationConfig** , zato so dodatki prikazani po pričakovanjih.

Ne priporočamo, da je parameter _Appsforofficeenabled_ nastavljen na **FALSE**. Vrednost **FALSE** preglasi vse zgoraj navedene nastavitve skrbniških in uporabniških vlog ter preprečuje, da bi kateri koli uporabnik v organizaciji aktiviral nove aplikacije.

Če želite več informacij, glejte [določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).