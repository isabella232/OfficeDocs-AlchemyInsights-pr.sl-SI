---
title: Dostop zavrnjen med ogledovanjem poteka dela
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688818"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="4c29f-102">Dostop zavrnjen med ogledovanjem poteka dela</span><span class="sxs-lookup"><span data-stu-id="4c29f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="4c29f-103">Poteki dela programa SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, ne morejo narediti sporočila o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na» vsi «.</span><span class="sxs-lookup"><span data-stu-id="4c29f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="4c29f-104">**Če želite odpraviti to težavo, naredite te korake:**</span><span class="sxs-lookup"><span data-stu-id="4c29f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="4c29f-105">Dovolite vsem, da si ogledajo člane SharePointove skupine.</span><span class="sxs-lookup"><span data-stu-id="4c29f-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="4c29f-106">Odstranite SharePointovo skupino iz vrstice» za «ali» Kp «v e-poštnem sporočilu.</span><span class="sxs-lookup"><span data-stu-id="4c29f-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="4c29f-107">Eksplicitno Dodajanje uporabnikov v vrstico» za «ali» Kp «, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.</span><span class="sxs-lookup"><span data-stu-id="4c29f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="4c29f-108">Če si želite ogledati več podrobnosti, se obrnite na [http nepooblaščeno za/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="4c29f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  