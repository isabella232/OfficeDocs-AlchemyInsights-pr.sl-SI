---
title: Indikatorji ne delujejo z brskalnikom Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676467"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="d7746-102">Indikatorji ne delujejo z brskalnikom Edge</span><span class="sxs-lookup"><span data-stu-id="d7746-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="d7746-103">Ko ustvarite indikator, ga Edge ne spoštuje (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="d7746-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="d7746-104">Če želite več informacij, [glejte Ustvarjanje indikatorjev za NASLOVE IP in URL-je/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="d7746-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="d7746-105">1. korak: Prepričajte se, da:</span><span class="sxs-lookup"><span data-stu-id="d7746-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="d7746-106">Preverite, ali je indikator pravilen (ni tipkarskih napak v NASLOVU IP, pravilno dejanje, pravilne skupine RBAC).</span><span class="sxs-lookup"><span data-stu-id="d7746-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="d7746-107">Ko ustvarite indikator, počakajte najmanj 2 uri, da upoštevate morebitno zakasnitev.</span><span class="sxs-lookup"><span data-stu-id="d7746-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="d7746-108">Preverite, ali so sistemi v Microsoft Defender for Endpoint zdaj na voljo.</span><span class="sxs-lookup"><span data-stu-id="d7746-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="d7746-109">Preverite, ali lahko sistem(i) komunicira z oblakom.</span><span class="sxs-lookup"><span data-stu-id="d7746-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="d7746-110">Preverite, ali je Smartscreen omogočen in dosegljiv, tako da se pomnete na [preskusno mesto](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="d7746-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="d7746-111">2. korak: Odpravljanje morebitne težave</span><span class="sxs-lookup"><span data-stu-id="d7746-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="d7746-112">Prepričajte se, da odjemalec izpolnjuje zahteve.</span><span class="sxs-lookup"><span data-stu-id="d7746-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="d7746-113">Če želite podrobnosti, [glejte Ustvarjanje indikatorjev za NASLOVE IP in URL-je/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="d7746-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="d7746-114">Preverite, ali uporabljate najnovejšo različico brskalnika Edge.</span><span class="sxs-lookup"><span data-stu-id="d7746-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="d7746-115">Če želite izvedeti, katero najnovejšo različico imate, [glejte Ugotovite, katero Microsoft Edge imate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="d7746-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="d7746-116">Znova zaženite brskalnik Edge.</span><span class="sxs-lookup"><span data-stu-id="d7746-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="d7746-117">Premaknite se na mesto, za katerega ste nastavitvijo indikator.</span><span class="sxs-lookup"><span data-stu-id="d7746-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="d7746-118">Če mesto ni prikazano v skladu s pričakovanji, nadaljujte s 3. korakom.</span><span class="sxs-lookup"><span data-stu-id="d7746-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="d7746-119">3. korak: Zbiranje podatkov</span><span class="sxs-lookup"><span data-stu-id="d7746-119">Step 3: Collect data</span></span>

- <span data-ttu-id="d7746-120">**Zberite diagnostične podatke MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="d7746-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="d7746-121">Navodila najdete v članku [Težave s računalniki za namestitev v Microsoft Defender za končno točko.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="d7746-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="d7746-122">Če vam je všeč namestitev in zbiranje sledenja aplikaciji Fiddler, glejte [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="d7746-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="d7746-123">Če raje uporabljate navodila Microsoftove podpore, izberite spodnjo ikono podpora, da odprete primer podpore.</span><span class="sxs-lookup"><span data-stu-id="d7746-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
