---
title: Dynamics 365 – napačna Nadzorna plošča v dinamiki 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711291"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="5217b-102">Napačna Nadzorna plošča v sistemu Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="5217b-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="5217b-103">Obstaja več razlogov, zakaj se lahko prikaže druga Nadzorna plošča, kot je tista, ki jo pričakujete:</span><span class="sxs-lookup"><span data-stu-id="5217b-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="5217b-104">Uporabnik je nastavil privzeto nadzorno ploščo uporabnika</span><span class="sxs-lookup"><span data-stu-id="5217b-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="5217b-105">Običajno lahko prepoznate privzeto nadzorno ploščo uporabnika, če gumb» **Nastavi kot privzeto** «ni prikazan v ukazni vrstici nadzorne plošče.</span><span class="sxs-lookup"><span data-stu-id="5217b-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="5217b-106">Privzeta Nadzorna plošča uporabnika bo preglasila vse druge privzete nadzorne plošče, tudi če uporabnikove privzete nadzorne plošče ni v trenutni aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="5217b-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="5217b-107">Če želite izključiti privzeto nadzorno ploščo, uporabite to nadomestno rešitev.</span><span class="sxs-lookup"><span data-stu-id="5217b-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="5217b-108">Ustvarite novo osebno nadzorno ploščo.</span><span class="sxs-lookup"><span data-stu-id="5217b-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="5217b-109">Nastavite to novo nadzorno ploščo kot privzeti uporabnik.</span><span class="sxs-lookup"><span data-stu-id="5217b-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="5217b-110">Izbrišite to nadzorno ploščo.</span><span class="sxs-lookup"><span data-stu-id="5217b-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="5217b-111">Nadzorna plošča je nastavljena v kazalo</span><span class="sxs-lookup"><span data-stu-id="5217b-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="5217b-112">Morda ste nastavili privzeto nadzorno ploščo organizacije tako, da izberete nadzorno ploščo in izberete možnost» Nastavi kot privzeto «v razdelku» prilagodi sistem «.</span><span class="sxs-lookup"><span data-stu-id="5217b-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="5217b-113">Nadzorna plošča, ki je opredeljena v Oblikovalniku zemljevida sitemap, bo imela prednost pred to nadzorno ploščo, če ima uporabnik dostop do njega.</span><span class="sxs-lookup"><span data-stu-id="5217b-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="5217b-114">Če želite, da uporabniki vidijo nadzorno ploščo, ki ste jo nastavili kot privzeto organizacijo, lahko naredite to:</span><span class="sxs-lookup"><span data-stu-id="5217b-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="5217b-115">Nastavitev nadzorne plošče v sitemap</span><span class="sxs-lookup"><span data-stu-id="5217b-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="5217b-116">Odstranjevanje dostopa do določene nadzorne plošče za kazalo za te uporabnike</span><span class="sxs-lookup"><span data-stu-id="5217b-116">Remove access to the sitemap defined dashboard for those users</span></span>
