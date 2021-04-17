---
title: Spreminjanje imenskih strežnikov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818628"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="2d006-102">Posodobite imenske strežnike tako, da bodo kazali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="2d006-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="2d006-103">Opomba: preteče lahko do 48 ur, preden bodo spremembe imenskega strežnika uporabljene.</span><span class="sxs-lookup"><span data-stu-id="2d006-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="2d006-104">Če želite nastaviti domeno v okolju Microsoft 365, morate posodobiti imenske strežnike v registratorju.</span><span class="sxs-lookup"><span data-stu-id="2d006-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="2d006-105">Ustvarjajte ali urejajte zapise imenskega strežnika v registratorju domene.</span><span class="sxs-lookup"><span data-stu-id="2d006-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="2d006-106">Pojdite na spletno mesto registratorja domene in poiščite mesto, kjer lahko urejate imenske strežnike.</span><span class="sxs-lookup"><span data-stu-id="2d006-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="2d006-107">Ustvarite ali uredite dva zapisa imenskega strežnika, da zagotovite ujemanje teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="2d006-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="2d006-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2d006-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="2d006-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2d006-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="2d006-110">Shranite spremembe.</span><span class="sxs-lookup"><span data-stu-id="2d006-110">Save changes.</span></span>

<span data-ttu-id="2d006-111">Podrobna navodila lahko najdete tudi v tem članku: [Sprememba imenskih strežnikov na poljubne registratorje domene](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="2d006-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  