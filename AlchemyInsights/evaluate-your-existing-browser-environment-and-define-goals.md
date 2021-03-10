---
title: Ocenjevanje obstoječega okolja brskalnika in določanje ciljev
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694821"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="e6913-102">Ocenjevanje obstoječega okolja brskalnika in določanje ciljev</span><span class="sxs-lookup"><span data-stu-id="e6913-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="e6913-103">Če ste vzeli čas za razumevanje trenutnega stanja brskalnika in projektne vizije, zagotovite, da so vse zainteresirane strani projekta poravnane in delujejo proti istemu cilju.</span><span class="sxs-lookup"><span data-stu-id="e6913-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="e6913-104">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="e6913-104">Follow these steps:</span></span>

1. <span data-ttu-id="e6913-105">Določite trenutno stanje.</span><span class="sxs-lookup"><span data-stu-id="e6913-105">Define your current state.</span></span> <span data-ttu-id="e6913-106">Razmislite o tem:</span><span class="sxs-lookup"><span data-stu-id="e6913-106">Consider the following:</span></span>
- <span data-ttu-id="e6913-107">Kateri brskalniki so trenutno razporejeni v vašem okolju?</span><span class="sxs-lookup"><span data-stu-id="e6913-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="e6913-108">Kateri brskalnik je nastavljen kot privzeti brskalnik?</span><span class="sxs-lookup"><span data-stu-id="e6913-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="e6913-109">Ali morate za nekatere aplikacije uporabljati Internet Explorer?</span><span class="sxs-lookup"><span data-stu-id="e6913-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="e6913-110">Ali uporabljate seznam mesta za podjetja v načinu za konfiguriranje Internet Explorerja danes?</span><span class="sxs-lookup"><span data-stu-id="e6913-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="e6913-111">Katere platforme OS, kot sta Windows 10 in macOS, podpira vaša okoljska podpora?</span><span class="sxs-lookup"><span data-stu-id="e6913-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="e6913-112">Katera orodja za upravljanje uporabljate za upravljanje brskalnika?</span><span class="sxs-lookup"><span data-stu-id="e6913-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="e6913-113">Kdo je odgovoren za konfiguracijo in upravljanje brskalnika?</span><span class="sxs-lookup"><span data-stu-id="e6913-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="e6913-114">Kakšen je postopek za preverjanje združljivosti brskalnika?</span><span class="sxs-lookup"><span data-stu-id="e6913-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="e6913-115">Določite cilje za uvajanje.</span><span class="sxs-lookup"><span data-stu-id="e6913-115">Define the goals for your deployment.</span></span> <span data-ttu-id="e6913-116">Upoštevajte te stvari:</span><span class="sxs-lookup"><span data-stu-id="e6913-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="e6913-117">Ali želite [nastaviti Microsoft Edge kot privzeti brskalnik](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span><span class="sxs-lookup"><span data-stu-id="e6913-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="e6913-118">Ali želite skriti starejšo različico Microsoft Edge ali želite, da [jo pustite na voljo za uporabnike](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span><span class="sxs-lookup"><span data-stu-id="e6913-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="e6913-119">Kako boste [konfigurirali Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span><span class="sxs-lookup"><span data-stu-id="e6913-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="e6913-120">Katere funkcije so kritične, da jih konfigurirate kot del začetne uvedbe?</span><span class="sxs-lookup"><span data-stu-id="e6913-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="e6913-121">Kakšen je postopek za obravnavanje vseh ugotovljenih težav z združljivostjo ali konfiguracijo?</span><span class="sxs-lookup"><span data-stu-id="e6913-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="e6913-122">Upoštevajte pogoje za funkcije, ki jih boste morda želeli uporabiti, na primer:</span><span class="sxs-lookup"><span data-stu-id="e6913-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="e6913-123">Aplikacija Windows Defender Guard</span><span class="sxs-lookup"><span data-stu-id="e6913-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="e6913-124">Način Internet Explorerja</span><span class="sxs-lookup"><span data-stu-id="e6913-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="e6913-125">Preverjanje pristnosti in sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="e6913-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="e6913-126">Ko dokončate te korake, ste pripravljeni na začetek načrtovanja strategije uvajanja.</span><span class="sxs-lookup"><span data-stu-id="e6913-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
