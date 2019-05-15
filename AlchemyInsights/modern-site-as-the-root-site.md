---
title: Sodobno mesto kot korensko mesto
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057775"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="97066-102">Sodobno mesto kot korensko mesto</span><span class="sxs-lookup"><span data-stu-id="97066-102">Modern site as root site</span></span>

<span data-ttu-id="97066-103">[Ciljna javnost](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) stranke moči zdaj usposobiti sodobnih komunikacijskih mesta izkušnje na klasični korensko mesto svoje SharePoint najemnik.</span><span class="sxs-lookup"><span data-stu-id="97066-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="97066-104">To funkcijo lahko aktivirate tako, da zaženete enostavno PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="97066-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="97066-105">O uspešni izvedbi PowerShell zapoved(), korensko mesto bo novo sporočilo strani domača stran.</span><span class="sxs-lookup"><span data-stu-id="97066-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="97066-106">Podrobnosti o zahtevah PowerShell cmdlet in funkcije so na voljo v članku [Omogoči-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="97066-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="97066-107">Mi boste se postopoma valjanje tole, off privzeto ciljno javnost strankam v začetku maja 2019, in izkotaliti se bo na voljo po vsem svetu do konca junija 2019.</span><span class="sxs-lookup"><span data-stu-id="97066-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="97066-108">Še naprej se nanašajo na [Vest središče](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) za druge nove funkcije z moderno.</span><span class="sxs-lookup"><span data-stu-id="97066-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="97066-109">**Pomembno**: ne izbrisati vaš vzoren korensko mesto ustvariti mesto sodobne komunikacije.</span><span class="sxs-lookup"><span data-stu-id="97066-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="97066-110">To je ne podpira Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97066-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="97066-111">Brisanje korenskega mesta bo vsa SharePointova mesta v organizaciji nedostopen za vse uporabnike, dokler obnovitev mesta ali ustvarite novo mesto na istem spletnem naslovu.</span><span class="sxs-lookup"><span data-stu-id="97066-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 