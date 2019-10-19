---
title: Dynamics 365-napačna Nadzorna plošča kaže v Dynamics 365 poenoteni vmesnik
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528567"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="acfc9-102">Napačna Nadzorna plošča je prikazana v poenotenem vmesniku Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="acfc9-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="acfc9-103">Obstaja več razlogov, zakaj se lahko prikaže drugačna Nadzorna plošča kot tista, ki jo pričakujete:</span><span class="sxs-lookup"><span data-stu-id="acfc9-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="acfc9-104">Uporabnik je nastavil privzeto nadzorno ploščo uporabnika</span><span class="sxs-lookup"><span data-stu-id="acfc9-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="acfc9-105">Značilno je, da lahko prepoznate uporabniško privzeto nadzorno ploščo je nastavljena, če se **Nastavi kot privzeto** gumb ne prikaže v ukazni vrstici nadzorne plošče.</span><span class="sxs-lookup"><span data-stu-id="acfc9-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="acfc9-106">Privzeta Nadzorna plošča za uporabnika bo preglasitev vseh drugih privzetih nadzornih plošč, tudi če uporabnikova privzeta Nadzorna plošča ni v trenutni aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="acfc9-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="acfc9-107">Če želite razdružiti privzeto nadzorno ploščo, uporabite to rešitev.</span><span class="sxs-lookup"><span data-stu-id="acfc9-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="acfc9-108">Ustvarite novo osebno nadzorno ploščo.</span><span class="sxs-lookup"><span data-stu-id="acfc9-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="acfc9-109">Nastavite novo nadzorno ploščo kot privzeti uporabnik.</span><span class="sxs-lookup"><span data-stu-id="acfc9-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="acfc9-110">Izbrišite nadzorno ploščo.</span><span class="sxs-lookup"><span data-stu-id="acfc9-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="acfc9-111">Nadzorna plošča je nastavljena na kazalo</span><span class="sxs-lookup"><span data-stu-id="acfc9-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="acfc9-112">Morda ste nastavili privzeto nadzorno ploščo organizacije tako, da izberete nadzorno ploščo in izberete» Nastavi kot privzeto «pod možnostjo» prilagodi sistem «.</span><span class="sxs-lookup"><span data-stu-id="acfc9-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="acfc9-113">Vendar pa bo Nadzorna plošča, določena v Oblikovalniku kazalo, prevladala nad to nadzorno ploščo, če ima uporabnik dostop do njega.</span><span class="sxs-lookup"><span data-stu-id="acfc9-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="acfc9-114">Če želite, da bodo uporabniki videli nadzorno ploščo, ki ste jo nastavili kot privzeto organizacijo, lahko:</span><span class="sxs-lookup"><span data-stu-id="acfc9-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="acfc9-115">Nastavitev nadzorne plošče na zemljevidu</span><span class="sxs-lookup"><span data-stu-id="acfc9-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="acfc9-116">Odstranitev dostopa do zemljevida, ki je določena za te uporabnike</span><span class="sxs-lookup"><span data-stu-id="acfc9-116">Remove access to the sitemap defined dashboard for those users</span></span>
