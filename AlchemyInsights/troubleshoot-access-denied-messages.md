---
title: Odpravljanje težav s postranski tajivec vest
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312680"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="496bc-102">Odpravljanje težav s postranski tajivec vest</span><span class="sxs-lookup"><span data-stu-id="496bc-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="496bc-p101">Če nekdo dobil sporočilo "Dostop zavrnjen" mapi v skupni rabi, lahko skrbnik zbirke mest omogočeno "dostop omejen uporabnik dovoljenje lockdown način." Vrteti to ne sveže:</span><span class="sxs-lookup"><span data-stu-id="496bc-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="496bc-105">Prebrskajte do mesta, kliknite ikono in nato kliknite **Nastavitve mesta**.</span><span class="sxs-lookup"><span data-stu-id="496bc-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="496bc-106">Odseku **Skrbništvo zbirke mest**kliknite **funkcije zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="496bc-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="496bc-107">Poleg **dostop omejen uporabnik dovoljenje lockdown način**, kliknite **Deactivate**.</span><span class="sxs-lookup"><span data-stu-id="496bc-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="496bc-p102">Postranski tajivec vest lahko pride tudi za mape v skupni rabi, če stran je mesta za objavljanje. Informacij, glejte [Dostop zavrnjen pri dostopu do mape v skupni rabi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="496bc-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="496bc-p103">Če je nekdo dobil sporočilo o napaki »Dostop zavrnjen« , ko poskušate ogledati zahteve za dostop, je treba dodati kot skrbnik zbirke mest ali član skupine lastnikov za mesto uporabnika. Za več informacij, glejte [Dostop zavrnjen dostop prošnja zapisati v seznam](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="496bc-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="496bc-112">Če uporabnik dobil sporočilo "Dostop zavrnjen", potem ko so bili odstranjeni iz krajevni imenik Active Directory in nato doda nazaj, glej [Dostop zavrnjen, ko uporabniški račun je sinhronizirana z Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="496bc-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

