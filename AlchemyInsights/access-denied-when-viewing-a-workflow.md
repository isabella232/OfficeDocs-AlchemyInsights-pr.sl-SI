---
title: Dostop zavrnjen pri ogledu poteka dela
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687346"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="2b321-102">Dostop zavrnjen pri ogledu poteka dela</span><span class="sxs-lookup"><span data-stu-id="2b321-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="2b321-103">Poteki dela SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, lahko spodleti s sporočilom o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na vsi.</span><span class="sxs-lookup"><span data-stu-id="2b321-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="2b321-104">**Če želite odpraviti to težavo, naredite naslednje:**</span><span class="sxs-lookup"><span data-stu-id="2b321-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="2b321-105">Dovolite vsem, da vidijo člane SharePointove skupine.</span><span class="sxs-lookup"><span data-stu-id="2b321-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="2b321-106">Odstranite SharePointovo skupino iz vrstice za ali CC e-poštnega sporočila.</span><span class="sxs-lookup"><span data-stu-id="2b321-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="2b321-107">Eksplicitno dodajte uporabnike v vrstico za ali CC, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.</span><span class="sxs-lookup"><span data-stu-id="2b321-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="2b321-108">Če si želite ogledati več podrobnosti, glejte [http nepooblaščeno, da/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="2b321-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  