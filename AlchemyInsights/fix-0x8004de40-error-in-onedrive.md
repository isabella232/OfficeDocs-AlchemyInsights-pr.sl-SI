---
title: Pritrditi zmota 0x8004de40 v OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133992"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b0df5-102">Pritrditi zmota 0x8004de40 v OneDrive</span><span class="sxs-lookup"><span data-stu-id="b0df5-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b0df5-103">Če prejmete napako 0x8004de40 z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b0df5-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b0df5-104">Odmevajoč vplivati računalo, medtem ko povezan z domeno dejvaen imenik.</span><span class="sxs-lookup"><span data-stu-id="b0df5-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b0df5-105">Če odmevajoč ne popraviti izdaja, ločiti in ponovno napravi iz sinje AD.</span><span class="sxs-lookup"><span data-stu-id="b0df5-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b0df5-106">**Opomba**: Bodite v omrežju podjetja med izvajanjem teh korakov.</span><span class="sxs-lookup"><span data-stu-id="b0df5-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b0df5-107">Ne izvede te korake, ko niste mogli vzpostaviti osrednjo infrastrukturo (na primer med potovanjem).</span><span class="sxs-lookup"><span data-stu-id="b0df5-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="b0df5-108">Plan visok zapoved uren.</span><span class="sxs-lookup"><span data-stu-id="b0df5-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="b0df5-109">Razkleniti visok zapoved uren, kliknite - **Start**, desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="b0df5-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="b0df5-110">Vrsto *dsregcmd /leave* in pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b0df5-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="b0df5-111">Ko končate, vnesite *dsregcmd/JOIN* in pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b0df5-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="b0df5-112">Ko končate, zaprite ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="b0df5-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="b0df5-113">Odmevajoč računalo, ter poleno v OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b0df5-113">Reboot the computer, and log into OneDrive.</span></span>