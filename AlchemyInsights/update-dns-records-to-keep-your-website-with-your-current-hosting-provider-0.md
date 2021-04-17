---
title: Posodabljanje zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827552"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b20cc-102">Posodabljanje zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja</span><span class="sxs-lookup"><span data-stu-id="b20cc-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b20cc-103">V Skrbniškem središču za Microsoft 365 pojdite na stran Nastavitve domen in na seznamu domen izberite domeno, ki jo uporabljate za spletno   >  [](https://admin.microsoft.com/Adminportal#/Domains) mesto.</span><span class="sxs-lookup"><span data-stu-id="b20cc-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="b20cc-104">Izberite **+ Nov zapis po** meri in vnesite to:</span><span class="sxs-lookup"><span data-stu-id="b20cc-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b20cc-105">Za **vrsto DNS** vnesite: A **(naslov)**</span><span class="sxs-lookup"><span data-stu-id="b20cc-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="b20cc-106">Za **Ime ali vzdevek gostitelja** vnesite to: **@**</span><span class="sxs-lookup"><span data-stu-id="b20cc-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="b20cc-107">Za **Naslov IP** vnesite statičen naslov IP za spletno mesto, kjer trenutno gostuje (na primer, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="b20cc-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="b20cc-108">To mora biti  *statični*  naslov IP za spletno mesto in ne  *dinamičen*  naslov IP.</span><span class="sxs-lookup"><span data-stu-id="b20cc-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="b20cc-109">Preverite, kje gostuje vaše spletno mesto, da boste lahko dobili statičen naslov IP za svoje javno spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="b20cc-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="b20cc-110">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="b20cc-110">Select **Save**.</span></span>

<span data-ttu-id="b20cc-111">Poleg tega lahko ustvarite zapis CNAME, da bodo stranke lahko pomagale najti vaše spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="b20cc-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b20cc-112">Izberite **+ Nov zapis po** meri in vnesite to:</span><span class="sxs-lookup"><span data-stu-id="b20cc-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b20cc-113">Za **vrsto DNS** vnesite: **CNAME (vzdevek)**</span><span class="sxs-lookup"><span data-stu-id="b20cc-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="b20cc-114">Za **Ime ali vzdevek gostitelja** vnesite to: **www**</span><span class="sxs-lookup"><span data-stu-id="b20cc-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="b20cc-115">V **polje Kaže na** naslov vnesite popolnoma določeno ime domene (FQDN) za spletno mesto (na primer contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b20cc-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="b20cc-116">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="b20cc-116">Select **Save**.</span></span>
