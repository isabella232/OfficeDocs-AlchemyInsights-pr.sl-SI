---
title: Omeji SharePoint Online na klasičen način
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369789"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c8fbf-102">Omeji SharePoint Online na klasičen način</span><span class="sxs-lookup"><span data-stu-id="c8fbf-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c8fbf-103">Nekatere organizacije še vedno zahtevajo izkušnje klasičen način.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c8fbf-104">Medtem ko obstajajo načrti umakniti klasičen način v a zrnast razina, je ni več mogoče omejiti celotno organizacijo (najemnik) na klasičen način za sezname in knjižnice.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c8fbf-105">Admin so naslednje možnosti za upravljanje posameznih seznami in knjižnice na klasičen način z uporabo granul neuporabe stikala, ki jih nudimo na naslednjih ravneh:</span><span class="sxs-lookup"><span data-stu-id="c8fbf-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c8fbf-106">zbirke mest</span><span class="sxs-lookup"><span data-stu-id="c8fbf-106">site collection</span></span>
- <span data-ttu-id="c8fbf-107">mesto</span><span class="sxs-lookup"><span data-stu-id="c8fbf-107">site</span></span>
- <span data-ttu-id="c8fbf-108">seznam</span><span class="sxs-lookup"><span data-stu-id="c8fbf-108">list</span></span>
- <span data-ttu-id="c8fbf-109">knjižnica</span><span class="sxs-lookup"><span data-stu-id="c8fbf-109">library</span></span>

<span data-ttu-id="c8fbf-110">Poleg tega seznamov, ki uporabljajo določene funkcije in prilagoditve, ki jih ne podpira sodobne bo še vedno samodejno preklopi na klasičen način.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c8fbf-111">Začetek aprila 1, 2019, proces v onesposobiti najemnik ravni odločijo iz sodobne seznam in knjižnice bo začeti in nadaljevati z maj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="c8fbf-112">Seznamov in knjižnic, ki so v klasičnem načinu zaradi najemnik opt-out, bo samodejno preusmeri do modernega.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="c8fbf-113">Če potrebujete klasičen način si oglejte več informacij [tukaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) in PnP Powershell navodila [tukaj](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) ki opisuje možnosti in orodja, ki jo lahko danes uporabljajo za uporabo na klasičen način izkušnje.</span><span class="sxs-lookup"><span data-stu-id="c8fbf-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
