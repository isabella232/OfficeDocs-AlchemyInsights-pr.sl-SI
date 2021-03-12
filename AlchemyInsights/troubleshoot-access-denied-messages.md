---
title: Odpravljanje težav z dostopom do zavrnjenih sporočil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704910"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="b860c-102">Odpravljanje težav z dostopom do zavrnjenih sporočil</span><span class="sxs-lookup"><span data-stu-id="b860c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="b860c-103">Če je nekdo dobil sporočilo» dostop zavrnjen «v mapo v skupni rabi v SharePointu, je morda skrbnik zbirke mest omogočil možnost» zaklep uporabniškega dovoljenja za omejeno dostopno «.</span><span class="sxs-lookup"><span data-stu-id="b860c-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="b860c-104">Če želite izklopiti to možnost:</span><span class="sxs-lookup"><span data-stu-id="b860c-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="b860c-105">Prebrskajte do mesta, kliknite ikono nastavitve in nato še **Nastavitve mesta**.</span><span class="sxs-lookup"><span data-stu-id="b860c-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="b860c-106">V razdelku **skrbništvo zbirke mest** kliknite **funkcije zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="b860c-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="b860c-107">Ob **možnosti zaklenjeni način dovoljenja za omejene uporabnike** kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="b860c-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="b860c-108">Sporočilo o zavrnjenem dostopu se lahko pojavi tudi v mapah v skupni rabi, če je mesto mesto za objavljanje.</span><span class="sxs-lookup"><span data-stu-id="b860c-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="b860c-109">Če želite več informacij, [si oglejte dostop zavrnjen, ko dostopate do mape v skupni rabi](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="b860c-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="b860c-110">Če je nekdo dobil sporočilo» dostop zavrnjen «, ko si želite ogledati zahteve za dostop, mora biti uporabnik dodan kot skrbnik zbirke mest ali član skupine lastnikov za mesto.</span><span class="sxs-lookup"><span data-stu-id="b860c-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="b860c-111">Če želite več informacij, glejte [seznam zavrnjenih dostop do zahtev za dostop](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="b860c-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="b860c-112">Če je uporabnik dobil sporočilo» dostop zavrnjen «, ko je bil odstranjen iz imenika Active Directory na mestu uporabe in ga nato dodal znova, si oglejte [dostop zavrnjen, ko je uporabniški račun sinhroniziran s storitvijo Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="b860c-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

