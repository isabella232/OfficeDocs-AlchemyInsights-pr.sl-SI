---
title: 'Odpravljanje težav z glasovno pošto '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679104"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="fdbe7-102">Odpravljanje težav z glasovno pošto</span><span class="sxs-lookup"><span data-stu-id="fdbe7-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="fdbe7-103">Zagotovite, da je funkcija zasedenosti zasedena namerno.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="fdbe7-104">Če ta funkcija ni potrebna za tega uporabnika:</span><span class="sxs-lookup"><span data-stu-id="fdbe7-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="fdbe7-105">Pojdite v [skrbniško središče za Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="fdbe7-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="fdbe7-106">V levem tiru se pomaknite na pravilnike **za klicanje** klicev v pravilniku za  >    >   **klicanje**.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="fdbe7-107">Izberite **upravljanje uporabnikov**.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="fdbe7-108">Poiščete uporabnika in spremenite pravilnik klicev na tistega, ki je **zaseden na zasedenem mestu, je na voljo, ko je klic** **izklopljen**.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="fdbe7-109">Kliknite **Uporabi**.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="fdbe7-110">Spremembe pravilnika lahko trajajo do 24 ur, da se replicirajo.</span><span class="sxs-lookup"><span data-stu-id="fdbe7-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="fdbe7-111">Če želite več informacij o tej funkciji, glejte: [zasedeno je na voljo med klicem](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="fdbe7-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
