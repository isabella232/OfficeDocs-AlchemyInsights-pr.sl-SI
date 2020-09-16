---
title: Omejevanje storitve SharePoint online v klasični način
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751438"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="92bca-102">Omejevanje storitve SharePoint online v klasični način</span><span class="sxs-lookup"><span data-stu-id="92bca-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="92bca-103">Nekatere organizacije še vedno zahtevajo klasično izkušnjo načina.</span><span class="sxs-lookup"><span data-stu-id="92bca-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="92bca-104">Čeprav ni načrtov za odstranjevanje klasičnega načina na ravni zrnatosti, ni več mogoče omejiti celotne organizacije (najemnika) v klasični način za sezname in knjižnice.</span><span class="sxs-lookup"><span data-stu-id="92bca-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="92bca-105">Skrbnik bo imel te možnosti za upravljanje posameznih seznamov in knjižnic v klasičnem načinu z uporabo neželenih stikal v granulah, ki jih nudimo na teh ravneh:</span><span class="sxs-lookup"><span data-stu-id="92bca-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="92bca-106">zbirka mest</span><span class="sxs-lookup"><span data-stu-id="92bca-106">site collection</span></span>
- <span data-ttu-id="92bca-107">mesta</span><span class="sxs-lookup"><span data-stu-id="92bca-107">site</span></span>
- <span data-ttu-id="92bca-108">seznam</span><span class="sxs-lookup"><span data-stu-id="92bca-108">list</span></span>
- <span data-ttu-id="92bca-109">knjižnica</span><span class="sxs-lookup"><span data-stu-id="92bca-109">library</span></span>

<span data-ttu-id="92bca-110">Poleg tega bodo seznami, ki uporabljajo določene funkcije in prilagoditve, ki jih sodobni ne podpirajo, še vedno samodejno preklopljeni v klasični način.</span><span class="sxs-lookup"><span data-stu-id="92bca-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="92bca-111">Začetek april 1, 2019, postopek za onemogočanje ravni najemnika, ki je izključena iz sodobnega seznama, in knjižnice se bodo zagnale in nadaljevale v maju 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="92bca-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="92bca-112">Seznami in knjižnice, ki so v klasičnem načinu zaradi izključitve najemnika, bodo samodejno premaknjeni v moderno.</span><span class="sxs-lookup"><span data-stu-id="92bca-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="92bca-113">Če potrebujete klasični način, si oglejte več informacij [tukaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) [in navodila za](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) uporabo storitve PnP PowerShell, ki opisujejo možnosti in orodja, ki jih lahko uporabite danes, da uporabite klasično izkušnjo načina.</span><span class="sxs-lookup"><span data-stu-id="92bca-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
