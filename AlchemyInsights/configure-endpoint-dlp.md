---
title: Konfiguracija končne točke za DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657945"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="e6b64-102">Konfiguracija končne točke za DLP</span><span class="sxs-lookup"><span data-stu-id="e6b64-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="e6b64-103">Microsoftova končna točka DLP omogoča razširitev zmogljivosti zaščite in nadzora DLP na občutljive informacije v napravah s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e6b64-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="e6b64-104">Ko so naprave nameščene v upravljanje naprav, lahko ustvarite pravilnike za zaščito pred zaščito elementov.</span><span class="sxs-lookup"><span data-stu-id="e6b64-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="e6b64-105">Raziskovalca dejavnosti je mogoče uporabiti za nadzor dejavnosti za občutljive elemente.</span><span class="sxs-lookup"><span data-stu-id="e6b64-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="e6b64-106">Če želite več informacij, glejte [Prenosne naprave v naprave za upravljanje](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="e6b64-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="e6b64-107">Če želite začeti uporabljati DLP končne točke:</span><span class="sxs-lookup"><span data-stu-id="e6b64-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="e6b64-108">Zagotovite, da imate ustrezno inventarno številko/naročnino za licenciranje.</span><span class="sxs-lookup"><span data-stu-id="e6b64-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="e6b64-109">Če želite več informacij, glejte [inventarna številka/licence](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="e6b64-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="e6b64-110">Preverite dovoljenja, ki so zahtevana za upravljanje naprave, dostop do strani za omogočanje ali vklop/izklop nadzora naprave.</span><span class="sxs-lookup"><span data-stu-id="e6b64-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="e6b64-111">Če želite več informacij, glejte razdelek [Dodelitev licenc](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="e6b64-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="e6b64-112">V upravljanje naprav lahko vklopite naprave tako, da upoštevate postopek za prenosne naprave.</span><span class="sxs-lookup"><span data-stu-id="e6b64-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="e6b64-113">Če želite več informacij, [informacije o](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="e6b64-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="e6b64-114">Ustvarite pravilnike OLP za zaščito občutljivih elementov.</span><span class="sxs-lookup"><span data-stu-id="e6b64-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="e6b64-115">Če želite več informacij, glejte [scenarijev pravilnika o zakasnitve](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="e6b64-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="e6b64-116">Če želite več informacij o preprečevanju izgube podatkov za Microsoft Endpoint DLP, glejte [Več informacij o preprečili izgube podatkov za končne točke storitve Microsoft 365 (predogled)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="e6b64-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="e6b64-117">**Pomembni koraki za zbiranje podatkov, če je potrebna podpora:**</span><span class="sxs-lookup"><span data-stu-id="e6b64-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="e6b64-118">Prenesite [predogled odjemalca MDATP Analyzer Preview.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="e6b64-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="e6b64-119">Zaženite orodje kot skrbnik v oknu »cmd«:</span><span class="sxs-lookup"><span data-stu-id="e6b64-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="e6b64-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="e6b64-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="e6b64-121">Ko ste pozvani **z vnesite število minut za zbiranje sledenj:**, vnesite število minut, zahtevanih za zagon scenarija.</span><span class="sxs-lookup"><span data-stu-id="e6b64-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="e6b64-122">Zaženite scenarij.</span><span class="sxs-lookup"><span data-stu-id="e6b64-122">Run the scenario.</span></span>

<span data-ttu-id="e6b64-123">Zberite rezultat datoteke Zip, ki ga daste posredniku za podporo.</span><span class="sxs-lookup"><span data-stu-id="e6b64-123">Collect the Zip file output to give to the Support agent.</span></span>
