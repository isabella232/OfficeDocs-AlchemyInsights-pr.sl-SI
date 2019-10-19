---
title: Sinhronizacija profila
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554349"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7729d-102">Kdaj se moj profil spremeni v sinhronizacijo s programom SharePoint User profile?</span><span class="sxs-lookup"><span data-stu-id="7729d-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7729d-103">SharePoint online uporablja posel razporejevalnika uvoza imenika Active Directory (uvoz oglasa) za uvoz uporabnikov in skupin v aplikacijo uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="7729d-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7729d-104">Uvoz oglasov sinhronizira spremembe iz trgovine SharePoint online Directory v aplikacijo uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="7729d-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="7729d-105">Te spremembe se obdelujejo v serijah.</span><span class="sxs-lookup"><span data-stu-id="7729d-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7729d-106">Posel razporejevalnika se zažene, dokler se spremembe ne sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="7729d-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7729d-107">Čas, potreben za zagon posla, je odvisen od števila sprememb procesa.</span><span class="sxs-lookup"><span data-stu-id="7729d-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="7729d-108">Veliko število sprememb traja dlje.</span><span class="sxs-lookup"><span data-stu-id="7729d-108">A large number of changes takes longer.</span></span> <span data-ttu-id="7729d-109">Pogodba o ravni storitve (SLA) določa, da se bo sprememba uporabnika v SharePointovem spletnem imeniku odražala v aplikaciji uporabniškega profila v 24 urah.</span><span class="sxs-lookup"><span data-stu-id="7729d-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7729d-110">Več informacij o sinhronizaciji uporabniških profilov v spletnem mestu SharePoint online</span><span class="sxs-lookup"><span data-stu-id="7729d-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

