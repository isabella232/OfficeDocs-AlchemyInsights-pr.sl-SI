---
title: Omogočanje vdelovanje podedovanih pogovornih okna za odpiranje poročil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814280"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="1f9d0-102">Omogočanje vdelovanje podedovanih pogovornih okna za odpiranje poročil</span><span class="sxs-lookup"><span data-stu-id="1f9d0-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="1f9d0-103">**Težava**</span><span class="sxs-lookup"><span data-stu-id="1f9d0-103">**Symptom**</span></span>

<span data-ttu-id="1f9d0-104">Uporabniki ne morejo odpreti poročil.</span><span class="sxs-lookup"><span data-stu-id="1f9d0-104">Users are unable to open reports.</span></span> <span data-ttu-id="1f9d0-105">»Nekaj je šlo narobe.</span><span class="sxs-lookup"><span data-stu-id="1f9d0-105">"Something has gone wrong.</span></span> <span data-ttu-id="1f9d0-106">Za več informacij si preberite tehnične podrobnosti.«</span><span class="sxs-lookup"><span data-stu-id="1f9d0-106">Check technical details for more details."</span></span>

<span data-ttu-id="1f9d0-107">**Vzrok**</span><span class="sxs-lookup"><span data-stu-id="1f9d0-107">**Cause**</span></span>

<span data-ttu-id="1f9d0-108">Poročil ni mogoče naložiti v UCI z napako »Opis obrazca je »null« ali ni definiran.«</span><span class="sxs-lookup"><span data-stu-id="1f9d0-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="1f9d0-109">Za poročila v uporabniškem vmesniku še vedno potrebujete podedovana pogovorna okna, zato mora imeti sistem stranke omogočeno možnost *allowlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="1f9d0-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="1f9d0-110">**Rešitev**</span><span class="sxs-lookup"><span data-stu-id="1f9d0-110">**Solution**</span></span>

1. <span data-ttu-id="1f9d0-111">Pojdite na **Nastavitve >skrbniškega > sistemskih nastavitev > zavihek Splošno.**</span><span class="sxs-lookup"><span data-stu-id="1f9d0-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="1f9d0-112">Nastavitev »Omogoči vdelovanje določenih podedovanih pogovornih okna v odjemalcu brskalnika poenotenega vmesnika« na **Da.**</span><span class="sxs-lookup"><span data-stu-id="1f9d0-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
