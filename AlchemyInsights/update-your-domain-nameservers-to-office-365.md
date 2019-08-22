---
title: Posodobitev imenskih strežnikov domene za Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506063"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="0225e-102">Posodobitev imenskih strežnikov domene za Office 365</span><span class="sxs-lookup"><span data-stu-id="0225e-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="0225e-103">Opomba: preteče lahko do 48 ur, preden bodo spremembe imenskega strežnika uporabljene.</span><span class="sxs-lookup"><span data-stu-id="0225e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="0225e-104">Če želite nastaviti domeno v storitvi Office 365, morate posodobiti imenske strežnike v registratorju.</span><span class="sxs-lookup"><span data-stu-id="0225e-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="0225e-105">Ustvarjajte ali urejajte zapise imenskega strežnika v registratorju domene.</span><span class="sxs-lookup"><span data-stu-id="0225e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="0225e-106">Pojdite na spletno mesto registratorja domene in poiščite mesto, kjer lahko urejate imenske strežnike.</span><span class="sxs-lookup"><span data-stu-id="0225e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="0225e-107">Ustvarite ali uredite dva zapisa imenskega strežnika, da zagotovite ujemanje teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="0225e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="0225e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0225e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="0225e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0225e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="0225e-110">Shranite spremembe.</span><span class="sxs-lookup"><span data-stu-id="0225e-110">Save changes.</span></span>

<span data-ttu-id="0225e-111">Podrobna navodila lahko najdete tudi v tem članku: [Sprememba imenskih strežnikov za nastavitev storitve Office 365 na poljubne registratorje domene](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="0225e-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  