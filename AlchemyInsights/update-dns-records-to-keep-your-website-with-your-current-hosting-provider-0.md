---
title: Posodobite zapise DNS, da bo vaše spletno mesto s trenutnim ponudnikom gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665776"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="97ba0-102">Posodobite zapise DNS, da bo vaše spletno mesto s trenutnim ponudnikom gostovanja</span><span class="sxs-lookup"><span data-stu-id="97ba0-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="97ba0-103">V skrbniškem središču Microsoft 365 pojdite na stran z **nastavitvami**  >  [domen](https://portal.office.com/adminportal/home#/Domains) in na seznamu domen izberite domeno, ki jo uporabljate za spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="97ba0-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="97ba0-104">Izberite **+ nov zapis po meri** in vnesite naslednje:</span><span class="sxs-lookup"><span data-stu-id="97ba0-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="97ba0-105">Za **vrsto DNS** vnesite: **A (naslov)**</span><span class="sxs-lookup"><span data-stu-id="97ba0-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="97ba0-106">Za **ime gostitelja ali vzdevek**vnesite to:**@**</span><span class="sxs-lookup"><span data-stu-id="97ba0-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="97ba0-107">Za naslov **IP**vnesite statični naslov IP za spletno mesto, kjer je trenutno gostujoča (na primer 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="97ba0-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="97ba0-108">To mora biti *statični* naslov IP za spletno stran, ne *dinamični* IP naslov.</span><span class="sxs-lookup"><span data-stu-id="97ba0-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="97ba0-109">Preverite s strani, kjer je vaša spletna stran gostuje, da se prepričajte, da lahko dobite statični naslov IP za vašo javno spletno stran.</span><span class="sxs-lookup"><span data-stu-id="97ba0-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="97ba0-110">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="97ba0-110">Select **Save**.</span></span>

<span data-ttu-id="97ba0-111">Poleg tega lahko ustvarite zapis CNAME, ki bo strankam pomagal najti vaše spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="97ba0-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="97ba0-112">Izberite **+ nov zapis po meri** in vnesite naslednje:</span><span class="sxs-lookup"><span data-stu-id="97ba0-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="97ba0-113">Za **tip DNS** vnesite: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="97ba0-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="97ba0-114">Za **ime gostitelja ali vzdevek**vnesite to: **www**</span><span class="sxs-lookup"><span data-stu-id="97ba0-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="97ba0-115">Za **točke za naslov**vnesite popolnoma kvalificirano ime domene (FQDN) za vaše spletno mesto (na primer contoso.com).</span><span class="sxs-lookup"><span data-stu-id="97ba0-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="97ba0-116">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="97ba0-116">Select **Save**.</span></span>
