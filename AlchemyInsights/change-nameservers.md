---
title: Spreminjanje imenskih strežnikov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902945"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="700c7-102">Posodobitev imenskih strežnikov domene za Office 365</span><span class="sxs-lookup"><span data-stu-id="700c7-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="700c7-103">Opomba: preteče lahko do 48 ur, preden bodo spremembe imenskega strežnika uporabljene.</span><span class="sxs-lookup"><span data-stu-id="700c7-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="700c7-104">Če želite nastaviti domeno v storitvi Office 365, morate posodobiti imenske strežnike v registratorju.</span><span class="sxs-lookup"><span data-stu-id="700c7-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="700c7-105">Ustvarjajte ali urejajte zapise imenskega strežnika v registratorju domene.</span><span class="sxs-lookup"><span data-stu-id="700c7-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="700c7-106">Pojdite na spletno mesto registratorja domene in poiščite mesto, kjer lahko urejate imenske strežnike.</span><span class="sxs-lookup"><span data-stu-id="700c7-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="700c7-107">Ustvarite ali uredite dva zapisa imenskega strežnika, da zagotovite ujemanje teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="700c7-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="700c7-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="700c7-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="700c7-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="700c7-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="700c7-110">Shranite spremembe.</span><span class="sxs-lookup"><span data-stu-id="700c7-110">Save changes.</span></span>

<span data-ttu-id="700c7-111">Podrobna navodila lahko najdete tudi v tem članku: [Sprememba imenskih strežnikov za nastavitev storitve Office 365 na poljubne registratorje domene](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="700c7-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  