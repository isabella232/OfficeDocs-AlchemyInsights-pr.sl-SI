---
title: Odpravljanje težav s postranski tajivec vest
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500436"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1b0b4-102">Odpravljanje težav s postranski tajivec vest</span><span class="sxs-lookup"><span data-stu-id="1b0b4-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1b0b4-103">Če nekdo dobil sporočilo o napaki »Dostop zavrnjen« za mape v skupni rabi v SharePoint, lahko skrbnik zbirke mest omogočeno "dostop omejen uporabnik dovoljenje lockdown način."</span><span class="sxs-lookup"><span data-stu-id="1b0b4-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="1b0b4-104">Vrteti to ne sveže:</span><span class="sxs-lookup"><span data-stu-id="1b0b4-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="1b0b4-105">Prebrskajte do mesta, kliknite ikono in nato kliknite **Nastavitve mesta**.</span><span class="sxs-lookup"><span data-stu-id="1b0b4-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1b0b4-106">Odseku **Skrbništvo zbirke mest**kliknite **funkcije zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="1b0b4-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1b0b4-107">Poleg **dostop omejen uporabnik dovoljenje lockdown način**, kliknite **Deactivate**.</span><span class="sxs-lookup"><span data-stu-id="1b0b4-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1b0b4-108">Postranski tajivec vest lahko pride tudi za mape v skupni rabi, če stran je mesta za objavljanje.</span><span class="sxs-lookup"><span data-stu-id="1b0b4-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="1b0b4-109">Informacij, glejte [Dostop zavrnjen pri dostopu do mape v skupni rabi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="1b0b4-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="1b0b4-110">Če je nekdo dobil sporočilo o napaki »Dostop zavrnjen« , ko poskušate ogledati zahteve za dostop, je treba dodati kot skrbnik zbirke mest ali član skupine lastnikov za mesto uporabnika.</span><span class="sxs-lookup"><span data-stu-id="1b0b4-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="1b0b4-111">Za več informacij, glejte [Dostop zavrnjen dostop prošnja zapisati v seznam](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="1b0b4-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1b0b4-112">Če uporabnik dobil sporočilo "Dostop zavrnjen", potem ko so bili odstranjeni iz krajevni imenik Active Directory in nato doda nazaj, glej [Dostop zavrnjen, ko uporabniški račun je sinhronizirana z Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="1b0b4-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

