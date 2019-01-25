---
title: 902 (sinhronizacijske napake zaradi podvojenih predmetov)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29490417"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="51355-102">Sinhronizacijske napake zaradi podvojenih predmetov</span><span class="sxs-lookup"><span data-stu-id="51355-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="51355-103">Eno od teh sporočil o napaki lahko prejmete, ko konča sinhronizacija imenika:</span><span class="sxs-lookup"><span data-stu-id="51355-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="51355-104">Ni mogoče posodobiti ta predmet v Microsoft Online Services, ker teh atributov, ki so povezani s tem predmetom so vrednosti, ki lahko že povezano z drugim predmetom, v vaš tukajšnji naslovnik.</span><span class="sxs-lookup"><span data-stu-id="51355-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="51355-105">Sinhroniziranega predmeta z isto zastopstvo ogovor že obstaja v imeniku Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="51355-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="51355-106">Mogoče posodobiti ta predmet, ker teh atributov, ki so povezani s tem predmetom so vrednosti, ki lahko že povezano z drugim predmetom, v vaš tukajšnji naslovnik storitve: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="51355-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="51355-107">Prepoznajte in odpravite težavo, prenesite in zaženite [Orodje za sanacijo IdFix DirSync napake](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="51355-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="51355-108">Če želite več informacij, glejte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="51355-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

