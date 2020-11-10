---
title: Pripombe na elemente seznama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982557"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="131ab-102">Pripombe na elemente seznama</span><span class="sxs-lookup"><span data-stu-id="131ab-102">Comments on List items</span></span>

<span data-ttu-id="131ab-103">Uporabniki bodo kmalu lahko dodali in izbrisali pripombe na elemente seznama.</span><span class="sxs-lookup"><span data-stu-id="131ab-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="131ab-104">Uporabniki si lahko ogledajo vse pripombe na element seznama in filtrirajo med pogledi, ki prikazujejo pripombe ali dejavnost, ki je povezana z elementom.</span><span class="sxs-lookup"><span data-stu-id="131ab-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="131ab-105">**Čas** :</span><span class="sxs-lookup"><span data-stu-id="131ab-105">**Timing** :</span></span>

<span data-ttu-id="131ab-106">**Ciljna izdaja** : postopno uvajanje sredi oktobra in predvidoma dokončano do sredine novembra</span><span class="sxs-lookup"><span data-stu-id="131ab-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="131ab-107">**Standardna izdaja** : postopno uvajanje sredi novembra in pričakovano dokončanje do začetka decembra</span><span class="sxs-lookup"><span data-stu-id="131ab-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="131ab-108">**Uvajanje** : ciljna izdaja za celotno organizacijo</span><span class="sxs-lookup"><span data-stu-id="131ab-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="131ab-109">Uporabniki morajo pred dodajanjem in brisanjem pripomb zabeležiti to:</span><span class="sxs-lookup"><span data-stu-id="131ab-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="131ab-110">Pripombe sledijo nastavitvam dovoljenj, ki so del SharePointa.</span><span class="sxs-lookup"><span data-stu-id="131ab-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="131ab-111">Klasični seznami, ki še niso zgrajeni za prikaz v sodobnih uporabniških vmesnikih, kot so seznami opravil, ne bodo imeli te funkcije komentiranja.</span><span class="sxs-lookup"><span data-stu-id="131ab-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="131ab-112">Komentiranje seznamov v aplikaciji Teams ni na voljo v tej izdaji.</span><span class="sxs-lookup"><span data-stu-id="131ab-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="131ab-113">Pripombe niso indeksirane z iskanjem.</span><span class="sxs-lookup"><span data-stu-id="131ab-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="131ab-114">Skrbniki lahko to funkcijo onemogočijo na ravni organizacije tako, da spremenite parameter **CommentsOnListItemsDisabled** v ukazu» cmdlet « **set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="131ab-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="131ab-115">Trenutno ni mogoče onemogočiti komentiranja na ravni mesta ali seznama.</span><span class="sxs-lookup"><span data-stu-id="131ab-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="131ab-116">Upamo, da bodo te kontrolnike v poznejši posodobitvi, verjetno v prvem četrtletju 2021.</span><span class="sxs-lookup"><span data-stu-id="131ab-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
