---
title: Konfiguracija DLP končne točke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556035"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="778b0-102">Konfiguracija DLP končne točke</span><span class="sxs-lookup"><span data-stu-id="778b0-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="778b0-103">Microsoft Endpoint DLP vam omogoča razširitev zaščite DLP in nadzora zmogljivosti za občutljive informacije v napravah s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="778b0-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="778b0-104">Ko so naprave v sistemu upravljanja, lahko ustvarite DLP pravilnike za uveljavitev zaščitnih dejanj na elementih.</span><span class="sxs-lookup"><span data-stu-id="778b0-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="778b0-105">Raziskovalca dejavnosti lahko uporabite za spremljanje dejavnosti za občutljive elemente.</span><span class="sxs-lookup"><span data-stu-id="778b0-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="778b0-106">Če želite več informacij, [glejte Naprave za vstavljanje v upravljanje naprav](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="778b0-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="778b0-107">Če želite začeti uporabljati DLP končne točke:</span><span class="sxs-lookup"><span data-stu-id="778b0-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="778b0-108">Poskrbite, da imate ustrezno licenco za enote skladiščenja/naročnine.</span><span class="sxs-lookup"><span data-stu-id="778b0-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="778b0-109">Če želite več informacij, [glejte Licenca za enote skladiščenja/naročnine](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="778b0-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="778b0-110">Preverite dovoljenja, ki so potrebna za omogočanje upravljanja naprav, dostopa do strani za vklop ali vklop/izklop nadzora naprave.</span><span class="sxs-lookup"><span data-stu-id="778b0-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="778b0-111">Če želite več informacij, [glejte Dovoljenja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="778b0-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="778b0-112">Naprave za upravljanje naprav v vozilu v skladu s postopkom naprav za vneti.</span><span class="sxs-lookup"><span data-stu-id="778b0-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="778b0-113">Če v razdelku Nastavitve skladnosti s predpisi M365 **Settings**manjka možnost »Naprava na krovu ( predogled),potrdite, da imate zgoraj navedeno ustrezno licenco in dovoljenja.</span><span class="sxs-lookup"><span data-stu-id="778b0-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="778b0-114">Če želite več informacij, [glejte Naprave za vstavljanje](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="778b0-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="778b0-115">Ustvarite pravilnike DLP za zaščito občutljivih elementov.</span><span class="sxs-lookup"><span data-stu-id="778b0-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="778b0-116">Če želite več informacij, [glejte Scenariji pravilnika DLP končne točke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="778b0-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="778b0-117">Če želite več informacij o programu Microsoft Endpoint DLP, glejte [Več o preprečevanju izgube podatkov (predogled) za Microsoft 365 Endpoint](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="778b0-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>