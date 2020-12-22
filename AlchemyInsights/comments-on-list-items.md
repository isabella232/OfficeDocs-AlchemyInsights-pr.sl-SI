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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724170"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="8f0c6-102">Pripombe na elemente seznama</span><span class="sxs-lookup"><span data-stu-id="8f0c6-102">Comments on List items</span></span>

<span data-ttu-id="8f0c6-103">Uporabniki si lahko ogledajo vse pripombe na element seznama in filtrirajo med pogledi, ki prikazujejo pripombe ali dejavnost, ki je povezana z elementom.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="8f0c6-104">Uporabniki morajo pred dodajanjem in brisanjem pripomb zabeležiti to:</span><span class="sxs-lookup"><span data-stu-id="8f0c6-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="8f0c6-105">Pripombe sledijo nastavitvam dovoljenj, ki so del SharePointa.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="8f0c6-106">Klasični seznami, ki še niso zgrajeni za prikaz v sodobnih uporabniških vmesnikih, kot so seznami opravil, ne bodo imeli te funkcije komentiranja.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="8f0c6-107">Komentiranje seznamov v aplikaciji Teams ni na voljo v tej izdaji.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="8f0c6-108">Pripombe niso indeksirane z iskanjem.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="8f0c6-109">Skrbniki lahko to funkcijo onemogočijo na ravni organizacije tako, da spremenite parameter **CommentsOnListItemsDisabled** v ukazu» cmdlet « **set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="8f0c6-110">Trenutno ni mogoče onemogočiti komentiranja na ravni mesta ali seznama.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="8f0c6-111">Upamo, da bodo te kontrolnike v poznejši posodobitvi, verjetno v prvem četrtletju 2021.</span><span class="sxs-lookup"><span data-stu-id="8f0c6-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
