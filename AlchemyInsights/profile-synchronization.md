---
title: Sinhronizacijo profila
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554349"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="b666c-102">Ko moje spremembe profil sinhronizacijo s programom SharePoint uporabniški profil?</span><span class="sxs-lookup"><span data-stu-id="b666c-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="b666c-103">SharePoint Online uporablja Active Directory uvoz posel razporejevalnika (AD uvoz) za uvoz uporabnikov in skupin v program uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="b666c-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="b666c-104">AD uvoz sinhronizira spremembe iz SharePoint Online imenik shrambe za program uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="b666c-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="b666c-105">Te spremembe se obdelujejo v svežnjih.</span><span class="sxs-lookup"><span data-stu-id="b666c-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="b666c-106">Zažene posel razporejevalnika, dokler spremembe sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="b666c-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="b666c-107">Čas, potreben zagon posla je odvisna od števila sprememb za obdelavo.</span><span class="sxs-lookup"><span data-stu-id="b666c-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="b666c-108">Številne spremembe traja dlje.</span><span class="sxs-lookup"><span data-stu-id="b666c-108">A large number of changes takes longer.</span></span> <span data-ttu-id="b666c-109">Sporazum za ravni storitev (SLA) navaja, da bo sprememba uporabnik v SharePoint Online Directory odraža v program uporabniškega profila v 24 urah.</span><span class="sxs-lookup"><span data-stu-id="b666c-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="b666c-110">Več informacij o sinhronizacija uporabniškega profila v SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b666c-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

