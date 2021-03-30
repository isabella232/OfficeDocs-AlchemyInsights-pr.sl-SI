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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402455"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="45d43-102">Konfiguracija končne točke za DLP</span><span class="sxs-lookup"><span data-stu-id="45d43-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="45d43-103">Microsoftova končna točka DLP omogoča razširitev zmogljivosti zaščite in nadzora DLP na občutljive informacije v napravah s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="45d43-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="45d43-104">Ko so naprave nameščene v upravljanje naprav, lahko ustvarite pravilnike za zaščito pred zaščito elementov.</span><span class="sxs-lookup"><span data-stu-id="45d43-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="45d43-105">Raziskovalca dejavnosti je mogoče uporabiti za nadzor dejavnosti za občutljive elemente.</span><span class="sxs-lookup"><span data-stu-id="45d43-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="45d43-106">Če želite več informacij, glejte [Prenosne naprave v naprave za upravljanje](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="45d43-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="45d43-107">Če želite začeti uporabljati DLP končne točke:</span><span class="sxs-lookup"><span data-stu-id="45d43-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="45d43-108">Zagotovite, da imate ustrezno inventarno številko/naročnino za licenciranje.</span><span class="sxs-lookup"><span data-stu-id="45d43-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="45d43-109">Če želite več informacij, glejte [inventarna številka/licence](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="45d43-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="45d43-110">Preverite dovoljenja, ki so zahtevana za upravljanje naprave, dostop do strani za omogočanje ali vklop/izklop nadzora naprave.</span><span class="sxs-lookup"><span data-stu-id="45d43-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="45d43-111">Če želite več informacij, glejte razdelek [Dodelitev licenc](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="45d43-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="45d43-112">V upravljanje naprav lahko vklopite naprave tako, da upoštevate postopek za prenosne naprave.</span><span class="sxs-lookup"><span data-stu-id="45d43-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="45d43-113">Če možnost sprejemanja naprav (predogled) v razdelku »Nastavitve skladnosti s predpisi  **storitve M365«**, preverite, ali imate ustrezno licenco in dovoljenja zgoraj.</span><span class="sxs-lookup"><span data-stu-id="45d43-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="45d43-114">Če želite več informacij, [informacije o](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="45d43-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="45d43-115">Ustvarite pravilnike OLP za zaščito občutljivih elementov.</span><span class="sxs-lookup"><span data-stu-id="45d43-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="45d43-116">Če želite več informacij, glejte [scenarijev pravilnika o zakasnitve](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="45d43-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="45d43-117">Če želite več informacij o preprečevanju izgube podatkov za Microsoft Endpoint DLP, glejte [Več informacij o preprečili izgube podatkov za končne točke storitve Microsoft 365 (predogled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="45d43-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="45d43-118">**Pomembni koraki za zbiranje podatkov, če je potrebna podpora:**</span><span class="sxs-lookup"><span data-stu-id="45d43-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="45d43-119">Prenesite predogled analizatorja za odjemalca MDATP iz storitve [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="45d43-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="45d43-120">Zaženite orodje kot skrbnik v oknu »cmd«:</span><span class="sxs-lookup"><span data-stu-id="45d43-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="45d43-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="45d43-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="45d43-122">Ko ste pozvani z »Vnesite število minut za zbiranje sledenj: »vnesite število minut, potrebnih za zagon scenarija</span><span class="sxs-lookup"><span data-stu-id="45d43-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="45d43-123">Zaženite scenarij</span><span class="sxs-lookup"><span data-stu-id="45d43-123">Run the scenario</span></span>

<span data-ttu-id="45d43-124">Zberite izhod datoteke Zip, ki ga želite dati posredniku za podporo.</span><span class="sxs-lookup"><span data-stu-id="45d43-124">Collect the Zip file output to be given to the Support agent.</span></span>
