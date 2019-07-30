---
title: Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925301"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="ad119-102">Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja</span><span class="sxs-lookup"><span data-stu-id="ad119-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="ad119-103">Na [področje](https://portal.office.com/adminportal/home#/Domains) strani, domen, na seznamu izberite domeno uporabljate za vašo spletno stran.</span><span class="sxs-lookup"><span data-stu-id="ad119-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="ad119-104">**+ Nov zapis po meri** in vnesite naslednje:</span><span class="sxs-lookup"><span data-stu-id="ad119-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ad119-105">Za **DNS vrsta** vnesite: **(naslov)**</span><span class="sxs-lookup"><span data-stu-id="ad119-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="ad119-106">**Ime gostitelja ali Alias**, vnesite naslednje:**@**</span><span class="sxs-lookup"><span data-stu-id="ad119-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="ad119-107">Za **IP naslov**, vnesite statični naslov IP za vašo spletno stran, kjer je trenutno gosti (npr. 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="ad119-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="ad119-108">To mora biti *statični* naslov IP za spletno stran, ne *dinamični* IP naslov.</span><span class="sxs-lookup"><span data-stu-id="ad119-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="ad119-109">Preveriti s mesto, kjer vašo spletno stran gostuje prepričati se lahko dobite statični naslov IP za javne spletne strani.</span><span class="sxs-lookup"><span data-stu-id="ad119-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="ad119-110">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="ad119-110">Select **Save**.</span></span>

<span data-ttu-id="ad119-111">Poleg tega lahko ustvarite zapis CNAME za pomoč uporabniki našli vašo spletno stran.</span><span class="sxs-lookup"><span data-stu-id="ad119-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="ad119-112">**+ Nov zapis po meri** in vnesite naslednje:</span><span class="sxs-lookup"><span data-stu-id="ad119-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ad119-113">Za **DNS vrsta** vnesite: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="ad119-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="ad119-114">**Ime gostitelja ali Alias**, vnesite naslednje: **www**</span><span class="sxs-lookup"><span data-stu-id="ad119-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="ad119-115">Za **točki naslov**, vnesite ime domene (FQDN) za vašo spletno stran (na primer contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ad119-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="ad119-116">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="ad119-116">Select **Save**.</span></span>
