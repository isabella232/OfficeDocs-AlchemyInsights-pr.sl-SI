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
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761775"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="e09fb-102">Omeji SharePoint Online na klasičen način</span><span class="sxs-lookup"><span data-stu-id="e09fb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="e09fb-103">Nekatere organizacije še vedno zahtevajo izkušnje klasičen način.</span><span class="sxs-lookup"><span data-stu-id="e09fb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="e09fb-104">Medtem ko obstajajo načrti umakniti klasičen način v a zrnast razina, je ni več mogoče omejiti celotno organizacijo (najemnik) na klasičen način za sezname in knjižnice.</span><span class="sxs-lookup"><span data-stu-id="e09fb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="e09fb-105">Admin so naslednje možnosti za upravljanje posameznih seznami in knjižnice na klasičen način z uporabo granul neuporabe stikala, ki jih nudimo na naslednjih ravneh:</span><span class="sxs-lookup"><span data-stu-id="e09fb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="e09fb-106">zbirke mest</span><span class="sxs-lookup"><span data-stu-id="e09fb-106">site collection</span></span>
- <span data-ttu-id="e09fb-107">mesto</span><span class="sxs-lookup"><span data-stu-id="e09fb-107">site</span></span>
- <span data-ttu-id="e09fb-108">seznam</span><span class="sxs-lookup"><span data-stu-id="e09fb-108">list</span></span>
- <span data-ttu-id="e09fb-109">knjižnica</span><span class="sxs-lookup"><span data-stu-id="e09fb-109">library</span></span>

<span data-ttu-id="e09fb-110">Poleg tega seznamov, ki uporabljajo določene funkcije in prilagoditve, ki jih ne podpira sodobne bo še vedno samodejno preklopi na klasičen način.</span><span class="sxs-lookup"><span data-stu-id="e09fb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="e09fb-111">Začetek aprila 1, 2019, proces v onesposobiti najemnik ravni odločijo iz sodobne seznam in knjižnice bo začeti in nadaljevati z maj 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="e09fb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="e09fb-112">Seznamov in knjižnic, ki so v klasičnem načinu zaradi najemnik opt-out, bo samodejno preusmeri do modernega.</span><span class="sxs-lookup"><span data-stu-id="e09fb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="e09fb-113">Če potrebujete klasičen način si oglejte več informacij [tukaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) in PnP Powershell navodila [tukaj](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) ki opisuje možnosti in orodja, ki jo lahko danes uporabljajo za uporabo na klasičen način izkušnje.</span><span class="sxs-lookup"><span data-stu-id="e09fb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
