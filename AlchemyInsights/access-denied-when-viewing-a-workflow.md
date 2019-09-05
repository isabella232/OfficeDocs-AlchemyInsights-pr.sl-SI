---
title: Dostop zavrnjen pri ogledu poteka dela
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747764"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="4fcd5-102">Dostop zavrnjen pri ogledu poteka dela</span><span class="sxs-lookup"><span data-stu-id="4fcd5-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="4fcd5-103">Poteki dela SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, lahko spodleti s sporočilom o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na vsi.</span><span class="sxs-lookup"><span data-stu-id="4fcd5-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="4fcd5-104">**Če želite odpraviti to težavo, naredite naslednje:**</span><span class="sxs-lookup"><span data-stu-id="4fcd5-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="4fcd5-105">Dovolite vsem, da vidijo člane SharePointove skupine.</span><span class="sxs-lookup"><span data-stu-id="4fcd5-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="4fcd5-106">Odstranite SharePointovo skupino iz vrstice za ali CC e-poštnega sporočila.</span><span class="sxs-lookup"><span data-stu-id="4fcd5-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="4fcd5-107">Eksplicitno dodajte uporabnike v vrstico za ali CC, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.</span><span class="sxs-lookup"><span data-stu-id="4fcd5-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="4fcd5-108">Če si želite ogledati več podrobnosti, glejte [http nepooblaščeno, da/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="4fcd5-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  