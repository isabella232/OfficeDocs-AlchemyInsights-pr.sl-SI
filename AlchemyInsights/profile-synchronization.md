---
title: Sinhronizacija profila
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768129"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="1850f-102">Kdaj se moj profil spremeni v sinhronizacijo s programom SharePoint User profile?</span><span class="sxs-lookup"><span data-stu-id="1850f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="1850f-103">SharePoint online uporablja posel razporejevalnika uvoza imenika Active Directory (uvoz oglasa) za uvoz uporabnikov in skupin v aplikacijo uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="1850f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="1850f-104">Uvoz oglasov sinhronizira spremembe iz trgovine SharePoint online Directory v aplikacijo uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="1850f-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="1850f-105">Te spremembe se obdelujejo v serijah.</span><span class="sxs-lookup"><span data-stu-id="1850f-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="1850f-106">Posel razporejevalnika se zažene, dokler se spremembe ne sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="1850f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1850f-107">Čas, potreben za zagon posla, je odvisen od števila sprememb procesa.</span><span class="sxs-lookup"><span data-stu-id="1850f-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="1850f-108">Veliko število sprememb traja dlje.</span><span class="sxs-lookup"><span data-stu-id="1850f-108">A large number of changes takes longer.</span></span> <span data-ttu-id="1850f-109">Pogodba o ravni storitve (SLA) določa, da se bo sprememba uporabnika v SharePointovem spletnem imeniku odražala v aplikaciji uporabniškega profila v 24 urah.</span><span class="sxs-lookup"><span data-stu-id="1850f-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="1850f-110">Več informacij o sinhronizaciji uporabniških profilov v spletnem mestu SharePoint online</span><span class="sxs-lookup"><span data-stu-id="1850f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

