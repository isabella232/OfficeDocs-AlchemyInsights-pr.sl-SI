---
title: Sinhronizacija profila
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801785"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a6939-102">Kdaj se moj profil spremeni tako, da se sinhronizira z aplikacijo SharePointovega uporabniškega profila?</span><span class="sxs-lookup"><span data-stu-id="a6939-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a6939-103">SharePoint online uporablja posel razporejevalnika za uvoz imenika Active Directory (uvoz oglasov) za uvoz uporabnikov in skupin v program uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="a6939-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a6939-104">Uvoz oglasov sinhronizira spremembe iz trgovine imenika SharePoint online v aplikacijo uporabniškega profila.</span><span class="sxs-lookup"><span data-stu-id="a6939-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a6939-105">Te spremembe so obdelane v svežnjih.</span><span class="sxs-lookup"><span data-stu-id="a6939-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a6939-106">Opravilo razporejevalnika se zažene, dokler se spremembe ne sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="a6939-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a6939-107">Čas trajanja posla je odvisen od števila sprememb, ki jih želite obdelati.</span><span class="sxs-lookup"><span data-stu-id="a6939-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a6939-108">Večje število sprememb traja dlje.</span><span class="sxs-lookup"><span data-stu-id="a6939-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a6939-109">Sporazum na ravni storitve (SLA) določa, da bo sprememba uporabnika v imeniku SharePoint Onlinea v programu uporabniškega profila prikazana v 24 urah.</span><span class="sxs-lookup"><span data-stu-id="a6939-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a6939-110">Več informacij o sinhronizaciji uporabniškega profila v storitvi SharePoint online</span><span class="sxs-lookup"><span data-stu-id="a6939-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

