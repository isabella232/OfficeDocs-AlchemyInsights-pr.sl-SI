---
title: Samodejno ustavitev sporočil iz selitve v Arhiv
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527116"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="a59e5-102">Samodejno ustavitev sporočil iz selitve v Arhiv</span><span class="sxs-lookup"><span data-stu-id="a59e5-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="a59e5-103">Če uporabljate pravilnik o hranjenju, lahko spremenite starost hranjenja v tem pravilniku, da preprečite samodejno arhiviranje sporočil.</span><span class="sxs-lookup"><span data-stu-id="a59e5-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="a59e5-104">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="a59e5-104">Here's how:</span></span>

1. <span data-ttu-id="a59e5-105">V [skrbniškem središču za Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)izberite oznake za hranjenje **upravljanja skladnosti**  >  .</span><span class="sxs-lookup"><span data-stu-id="a59e5-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="a59e5-106">Poiščite svojo potezo v arhiviranju oznake hranjenja.</span><span class="sxs-lookup"><span data-stu-id="a59e5-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="a59e5-107">V oznaki za hranjenje spremenite obdobje hranjenja (obdobje arhiviranja), da **nikoli ne** ustavite samodejnega arhiviranja elementov s pravilnikom o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="a59e5-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="a59e5-108">S tem boste spremenili nastavitev arhiviranja za vse nabiralnike s to oznako za hranjenje.</span><span class="sxs-lookup"><span data-stu-id="a59e5-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
