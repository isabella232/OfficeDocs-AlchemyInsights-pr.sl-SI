---
title: Offboard, ki niso naprave s sistemom Windows, napredna zaščita pred grožnjami Microsoft Defender (ATP)
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
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695160"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="2e7c4-102">Offboard, ki niso naprave s sistemom Windows, napredna zaščita pred grožnjami Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="2e7c4-103">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="2e7c4-103">Here's how:</span></span>

1. <span data-ttu-id="2e7c4-104">Če želite izključiti rešitev tretje osebe v storitvi Microsoft Defender ATP, glejte dokumentacijo tretje osebe.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="2e7c4-105">Iz svojega najemnika storitve Azure Active Directory odstranite dovoljenja za rešitev tretje osebe:</span><span class="sxs-lookup"><span data-stu-id="2e7c4-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="2e7c4-106">Vpišite se v [portal Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="2e7c4-107">Izberite **vse storitve**  >  **Azure Active Directory**  >  **Enterprise aplikacije**.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="2e7c4-108">Izberite aplikacijo, ki jo želite offboard.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="2e7c4-109">Izberite **Izbriši**.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-109">Select **Delete**.</span></span>

<span data-ttu-id="2e7c4-110">Če želite izvedeti več, glejte [offboard naprave, ki niso v sistemu Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
