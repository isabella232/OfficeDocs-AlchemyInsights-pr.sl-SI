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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="efcb5-102">Več uporabnikov, ki ne vidijo dodatkov v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="efcb5-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="efcb5-103">Če preskusite dodatke Outlook in nobeden ne prikaže, kot prvi korak za odpravljanje težav, uporabite cmdlet **Get-OrganizationConfig** PowerShell za poizvedbo _Appsforofficeenabled_ parameter.</span><span class="sxs-lookup"><span data-stu-id="efcb5-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="efcb5-104">Če poizvedba vrne vrednost **FALSE**, nastavite ta parameter na **True** z ukazom» cmdlet « **Set-OrganizationConfig** , zato so dodatki prikazani po pričakovanjih.</span><span class="sxs-lookup"><span data-stu-id="efcb5-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="efcb5-105">Ne priporočamo, da je parameter _Appsforofficeenabled_ nastavljen na **FALSE**.</span><span class="sxs-lookup"><span data-stu-id="efcb5-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="efcb5-106">Vrednost **FALSE** preglasi vse zgoraj navedene nastavitve skrbniških in uporabniških vlog ter preprečuje, da bi kateri koli uporabnik v organizaciji aktiviral nove aplikacije.</span><span class="sxs-lookup"><span data-stu-id="efcb5-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="efcb5-107">Če želite več informacij, glejte [določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="efcb5-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>