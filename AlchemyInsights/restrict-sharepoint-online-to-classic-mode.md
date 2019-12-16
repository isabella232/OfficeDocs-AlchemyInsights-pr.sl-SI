---
title: Omejevanje spletnega mesta SharePoint online v klasični način
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048776"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="1c894-102">Omejevanje spletnega mesta SharePoint online v klasični način</span><span class="sxs-lookup"><span data-stu-id="1c894-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="1c894-103">Nekatere organizacije še vedno potrebujejo izkušnjo klasičnega načina.</span><span class="sxs-lookup"><span data-stu-id="1c894-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="1c894-104">Čeprav ni načrtov za odstranjevanje klasičnega načina na zrnat ravni, ni več mogoče omejiti celotne organizacije (najemnika) v klasični način za sezname in knjižnice.</span><span class="sxs-lookup"><span data-stu-id="1c894-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="1c894-105">Admin bo imel naslednje možnosti za upravljanje posameznih seznamov in knjižnic v klasičnem načinu z uporabo zrnat opt-out stikala, ki jih nudimo na naslednjih ravneh:</span><span class="sxs-lookup"><span data-stu-id="1c894-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="1c894-106">zbirka mest</span><span class="sxs-lookup"><span data-stu-id="1c894-106">site collection</span></span>
- <span data-ttu-id="1c894-107">Stran</span><span class="sxs-lookup"><span data-stu-id="1c894-107">site</span></span>
- <span data-ttu-id="1c894-108">Seznam</span><span class="sxs-lookup"><span data-stu-id="1c894-108">list</span></span>
- <span data-ttu-id="1c894-109">Knjižnica</span><span class="sxs-lookup"><span data-stu-id="1c894-109">library</span></span>

<span data-ttu-id="1c894-110">Poleg tega bodo seznami, ki uporabljajo določene funkcije in prilagoditve, ki jih sodobna ne podpira, še vedno samodejno preklopili v klasični način.</span><span class="sxs-lookup"><span data-stu-id="1c894-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="1c894-111">Začetek april 1, 2019, proces v onesposobiti najemnik razina izbirati izven Modern zapisati v seznam ter knjižničar hoteti začetek ter vzdržnost skozi maj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="1c894-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="1c894-112">Seznami in knjižnice, ki so v klasičnem načinu kot posledica zavrnitve najemnika, bodo samodejno premaknjene v moderno.</span><span class="sxs-lookup"><span data-stu-id="1c894-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="1c894-113">Če vi zahtevati vzoren način prosim zagledati več sporočilo [vsepovsod](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ter PnP PowerShell predpis [vsepovsod](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) to popisovati predkupna pravica ter rokodelsko orodje vi moči raba danes rabiti vzoren način doživetje.</span><span class="sxs-lookup"><span data-stu-id="1c894-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
