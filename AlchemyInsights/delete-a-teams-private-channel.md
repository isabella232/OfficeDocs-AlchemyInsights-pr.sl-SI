---
title: Brisanje zasebnega kanala »Teams]
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439914"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="5254b-102">Brisanje zasebnega kanala »Teams]</span><span class="sxs-lookup"><span data-stu-id="5254b-102">Delete a Teams private channel</span></span>

<span data-ttu-id="5254b-103">Microsoft se zaveda težave pri brisanju zasebnega kanala Teams, če imate omogočene SharePointove pravilnike o hranjenju za temeljno SharePointovo mesto.</span><span class="sxs-lookup"><span data-stu-id="5254b-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="5254b-104">Microsoft dela na popravku.</span><span class="sxs-lookup"><span data-stu-id="5254b-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="5254b-105">Medtem lahko zasebni kanal izbrišete s spodnjimi rešitvami.</span><span class="sxs-lookup"><span data-stu-id="5254b-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="5254b-106">**Izključite skupino/zbirko mest iz Pravilnika o hranjenju SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="5254b-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="5254b-107">Pojdite na skrbniški portal za Office 365 in v levem **podoknu za krmarjenje** izberite Pokaži vse.</span><span class="sxs-lookup"><span data-stu-id="5254b-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="5254b-108">V **razdelku Skrbniška**središča pojdite **na Pravilnik & za**preprečevanje  >  **izgube podatkov o**  >  **skladnosti**s predpisi .</span><span class="sxs-lookup"><span data-stu-id="5254b-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="5254b-109">Določite pravilnik, ki velja za SharePointova mesta, in spremenite pravilnik, tako da SharePointovo mesto za ekipo, ki vsebuje zasebni kanal, NI vključeno v pravilnik o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="5254b-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="5254b-110">Shranite pravilnik.</span><span class="sxs-lookup"><span data-stu-id="5254b-110">Save the policy.</span></span>
    <span data-ttu-id="5254b-111">Če nastavitve pravilnika začnejo veljati, lahko traja do 24 ur.</span><span class="sxs-lookup"><span data-stu-id="5254b-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="5254b-112">Ko je spletno mesto izključeno, lahko izbrišete zasebni kanal.</span><span class="sxs-lookup"><span data-stu-id="5254b-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="5254b-113">Zasebni ***kanal*** boste morda lahko izbrisali s programom Microsoft Teams v napravi Android.</span><span class="sxs-lookup"><span data-stu-id="5254b-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="5254b-114">Če želite povezane SharePointove informacije, [glejte Elementi v SharePoint Onlineu ali Storitvi OneDrive za podjetja niso uspeli izbrisati](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="5254b-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>