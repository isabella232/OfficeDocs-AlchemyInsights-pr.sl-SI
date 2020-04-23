---
title: Spreminjanje imenskih strežnikov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706771"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="de3eb-102">Posodobite imenske strežnike tako, da bodo kazali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="de3eb-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="de3eb-103">Opomba: preteče lahko do 48 ur, preden bodo spremembe imenskega strežnika uporabljene.</span><span class="sxs-lookup"><span data-stu-id="de3eb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="de3eb-104">Če želite nastaviti domeno v okolju Microsoft 365, morate posodobiti imenske strežnike v registratorju.</span><span class="sxs-lookup"><span data-stu-id="de3eb-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="de3eb-105">Ustvarjajte ali urejajte zapise imenskega strežnika v registratorju domene.</span><span class="sxs-lookup"><span data-stu-id="de3eb-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="de3eb-106">Pojdite na spletno mesto registratorja domene in poiščite mesto, kjer lahko urejate imenske strežnike.</span><span class="sxs-lookup"><span data-stu-id="de3eb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="de3eb-107">Ustvarite ali uredite dva zapisa imenskega strežnika, da zagotovite ujemanje teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="de3eb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="de3eb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="de3eb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="de3eb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="de3eb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="de3eb-110">Shranite spremembe.</span><span class="sxs-lookup"><span data-stu-id="de3eb-110">Save changes.</span></span>

<span data-ttu-id="de3eb-111">Podrobna navodila lahko najdete tudi v tem članku: [Sprememba imenskih strežnikov na poljubne registratorje domene](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="de3eb-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  