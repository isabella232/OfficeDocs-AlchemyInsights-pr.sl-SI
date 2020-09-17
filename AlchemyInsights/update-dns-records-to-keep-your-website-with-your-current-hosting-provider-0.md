---
title: Posodobitev zapisov DNS za ohranjanje spletnega mesta s trenutnim ponudnikom gostovanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815801"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="c6fb1-102">Posodobitev zapisov DNS za ohranjanje spletnega mesta s trenutnim ponudnikom gostovanja</span><span class="sxs-lookup"><span data-stu-id="c6fb1-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="c6fb1-103">V skrbniškem središču za Microsoft 365 pojdite na stran **Nastavitev**  >  [domen](https://admin.microsoft.com/Adminportal#/Domains) in na seznamu domen izberite domeno, ki jo uporabljate za spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="c6fb1-104">Izberite **+ nov zapis po meri** in vnesite to:</span><span class="sxs-lookup"><span data-stu-id="c6fb1-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c6fb1-105">Za **vrsto DNS** vnesite: **A (naslov)**</span><span class="sxs-lookup"><span data-stu-id="c6fb1-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="c6fb1-106">Za **ime ali vzdevek gostitelja**vnesite to: **@**</span><span class="sxs-lookup"><span data-stu-id="c6fb1-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="c6fb1-107">Za **naslov IP**vnesite statični naslov IP za spletno mesto, kjer trenutno gostuje (na primer: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="c6fb1-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="c6fb1-108">To mora biti  *statični*  naslov IP za spletno mesto, ne pa  *dinamični*  naslov IP.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="c6fb1-109">Obiščite spletno mesto, kjer gostuje spletno mesto, da se prepričate, da lahko dobite statični naslov IP za javno spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="c6fb1-110">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-110">Select **Save**.</span></span>

<span data-ttu-id="c6fb1-111">Poleg tega lahko ustvarite zapis CNAME za pomoč uporabnikom pri iskanju spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="c6fb1-112">Izberite **+ nov zapis po meri** in vnesite to:</span><span class="sxs-lookup"><span data-stu-id="c6fb1-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c6fb1-113">Za **vrsto DNS** vnesite: **CNAME (vzdevek)**</span><span class="sxs-lookup"><span data-stu-id="c6fb1-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="c6fb1-114">Za **ime ali vzdevek gostitelja**vnesite to: **www**</span><span class="sxs-lookup"><span data-stu-id="c6fb1-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="c6fb1-115">Za **točke na naslov**vnesite popolnoma določeno ime domene (FQDN) za vaše spletno mesto (na primer contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c6fb1-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="c6fb1-116">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="c6fb1-116">Select **Save**.</span></span>
