---
title: Podpora Microsoft Edge za aplikacijo Microsoft Defender Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584010"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="aa52a-102">Podpora Microsoft Edge za aplikacijo Microsoft Defender Guard</span><span class="sxs-lookup"><span data-stu-id="aa52a-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="aa52a-103">Program Guard, zasnovan za Windows 10 in Microsoft Edge, uporablja način za izolacijo strojne opreme, ki uporabniku omogoča krmarjenje do nezaupanja vrednega mesta znotraj izoliranega vsebnika Hyper-V – omogočeno, ločen od gostiteljskega operacijskega sistema.</span><span class="sxs-lookup"><span data-stu-id="aa52a-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="aa52a-104">Skrbnik podjetja definira seznam zaupanja vrednih spletnih mest, virov v oblaku in notranjih omrežij.</span><span class="sxs-lookup"><span data-stu-id="aa52a-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="aa52a-105">Ko uporabnik obišče mesto, ki ni na seznamu, bo Microsoft Edge odprl mesto v vsebniku.</span><span class="sxs-lookup"><span data-stu-id="aa52a-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="aa52a-106">To pomeni, da bo v primeru, če se mesto izkaže kot zlonamerno, gostiteljski računalnik ostal zaščiten in napadalec ne bo mogel priti do podatkov podjetja.</span><span class="sxs-lookup"><span data-stu-id="aa52a-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="aa52a-107">Namestitev pripon v vsebniku je podprta z različico Microsoft Edge 81, ki jo je mogoče nadzorovati prek pravilnika.</span><span class="sxs-lookup"><span data-stu-id="aa52a-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="aa52a-108">Naslov updateURL, ki se uporablja v pravilniku ExtensionInstallForcelist, je treba dodati kot nevtralni vir v pravilniku o izolaciji omrežja, ki ga uporablja skrbnik aplikacije.</span><span class="sxs-lookup"><span data-stu-id="aa52a-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="aa52a-109">Če želite več informacij, si oglejte [Microsoftova podpora za Microsoft Defender za aplikacijo Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="aa52a-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
