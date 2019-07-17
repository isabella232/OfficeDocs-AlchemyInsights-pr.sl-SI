---
title: Dynamics 365 - narobe armaturni plošči kaže v enotni vmesniku Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748759"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="636f7-102">Narobe armaturni plošči kaže v enotni vmesniku Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="636f7-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="636f7-103">Obstaja več razlogov, zakaj lahko vidite različne nadzorne plošče kot tisti, ki pričakujete:</span><span class="sxs-lookup"><span data-stu-id="636f7-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="636f7-104">Uporabnik je nastavite privzeti uporabniški nadzorni plošči</span><span class="sxs-lookup"><span data-stu-id="636f7-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="636f7-105">Običajno lahko prepoznavanje uporabnika privzeto nadzorno ploščo je nastavljena, če **Nastavite kot privzeti** gumb ne Prikaži v blatnik ukazno vrstico.</span><span class="sxs-lookup"><span data-stu-id="636f7-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="636f7-106">Privzete nadzorne plošče uporabnika bo razveljavila vse druge privzete nadzorne plošče, tudi če uporabnikove privzete nadzorne plošče ni v trenutni app.</span><span class="sxs-lookup"><span data-stu-id="636f7-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="636f7-107">Raba sledeč workaround v izključeno njihovo privzeto nadzorno ploščo.</span><span class="sxs-lookup"><span data-stu-id="636f7-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="636f7-108">Ustvarite novo osebno armaturno ploščo.</span><span class="sxs-lookup"><span data-stu-id="636f7-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="636f7-109">Nastavite to novo nadzorno ploščo kot uporabniško privzeto.</span><span class="sxs-lookup"><span data-stu-id="636f7-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="636f7-110">Brisanje te nadzorne plošče.</span><span class="sxs-lookup"><span data-stu-id="636f7-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="636f7-111">Armaturni plošči se nahaja v kazalo</span><span class="sxs-lookup"><span data-stu-id="636f7-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="636f7-112">Lahko nastavite za organizacijo privzeto nadzorno ploščo z izbiro nadzorno ploščo in izberete "Nastavi kot privzeto" pod "Šega sistem".</span><span class="sxs-lookup"><span data-stu-id="636f7-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="636f7-113">Vendar blatnik, opredeljen v kazalo oblikovalec hoteti zalotiti predhodnost nad to nadzorno ploščo, če uporabnik ima dostop do njega.</span><span class="sxs-lookup"><span data-stu-id="636f7-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="636f7-114">Da imajo uporabniki videli armaturni plošči, ki ste jo nastavili kot privzeti organizacije, lahko bodisi:</span><span class="sxs-lookup"><span data-stu-id="636f7-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="636f7-115">Nastavite to nadzorno ploščo v kazalo</span><span class="sxs-lookup"><span data-stu-id="636f7-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="636f7-116">Odstranjevanje dostopa do kazalo določene nadzorne plošče za tiste uporabnike</span><span class="sxs-lookup"><span data-stu-id="636f7-116">Remove access to the sitemap defined dashboard for those users</span></span>
