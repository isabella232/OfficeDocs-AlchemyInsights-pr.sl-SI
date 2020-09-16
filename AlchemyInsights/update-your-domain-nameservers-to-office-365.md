---
title: Posodobite imenske strežnike tako, da bodo kazali na Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734927"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="cc6c2-102">Posodobite imenske strežnike tako, da bodo kazali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="cc6c2-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="cc6c2-103">Opomba: preteče lahko do 48 ur, preden bodo spremembe imenskega strežnika uporabljene.</span><span class="sxs-lookup"><span data-stu-id="cc6c2-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="cc6c2-104">Če želite nastaviti domeno z Microsoftom, morate posodobiti imenske strežnike pri registratorju.</span><span class="sxs-lookup"><span data-stu-id="cc6c2-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="cc6c2-105">Ustvarjajte ali urejajte zapise imenskega strežnika v registratorju domene.</span><span class="sxs-lookup"><span data-stu-id="cc6c2-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="cc6c2-106">Pojdite na spletno mesto registratorja domene in poiščite mesto, kjer lahko urejate imenske strežnike.</span><span class="sxs-lookup"><span data-stu-id="cc6c2-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="cc6c2-107">Ustvarite ali uredite dva zapisa imenskega strežnika, da zagotovite ujemanje teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="cc6c2-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="cc6c2-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="cc6c2-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="cc6c2-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="cc6c2-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="cc6c2-110">Shranite spremembe.</span><span class="sxs-lookup"><span data-stu-id="cc6c2-110">Save changes.</span></span>

<span data-ttu-id="cc6c2-111">Podrobna navodila najdete tudi v tem članku: [Spreminjanje imenskih strežnikov za nastavitev storitve Microsoft 365 s katerim koli registratorjem domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="cc6c2-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  