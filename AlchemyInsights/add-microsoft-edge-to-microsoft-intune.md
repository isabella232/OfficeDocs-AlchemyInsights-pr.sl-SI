---
title: Dodajanje Microsoft Edge v Microsoft InTune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194576"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="a5f1d-102">Dodajanje Microsoft Edge v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="a5f1d-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="a5f1d-103">Če želite omogočiti uvajanje, konfiguriranje, nadzorovanje in zaščito Microsoft Edge za Windows 10, ga morate najprej dodati v Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="a5f1d-104">InTune podpira Microsoft Edge 77 in novejše različice.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="a5f1d-105">InTune bo zaznal vse že obstoječe naprave Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="a5f1d-106">Če je Microsoft Edge nameščen v uporabniškem kontekstu, bo sistemska namestitev prepisala namestitev v uporabniškem kontekstu.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="a5f1d-107">Če je Microsoft Edge nameščen v sistemskem kontekstu, bo poročilo o uspehu namestitve zabeleženo.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="a5f1d-108">Vnaprej nameščeni Microsoft Edge 77 in novejše različice, za vse kanale v uporabniškem kontekstu, bodo prepisani s programom Microsoft Edge, ki je nameščen v sistemskem kontekstu.</span><span class="sxs-lookup"><span data-stu-id="a5f1d-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="a5f1d-109">**Predpogoj**</span><span class="sxs-lookup"><span data-stu-id="a5f1d-109">**Prerequisite**</span></span>

<span data-ttu-id="a5f1d-110">Različica 1709 ali novejše različice sistema Windows 10</span><span class="sxs-lookup"><span data-stu-id="a5f1d-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="a5f1d-111">**Koraki za dodajanje roba v InTune**</span><span class="sxs-lookup"><span data-stu-id="a5f1d-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="a5f1d-112">[Konfiguracija programa v programu InTune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="a5f1d-113">[Konfigurirajte informacije o aplikaciji](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="a5f1d-114">[Konfiguracija nastavitev aplikacije](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="a5f1d-115">[Izberite oznake obsega (izbirno)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="a5f1d-116">[Dodajte aplikacijo](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="a5f1d-117">Če želite več informacij, glejte [Odpravljanje težav](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a5f1d-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




