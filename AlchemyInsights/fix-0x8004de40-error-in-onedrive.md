---
title: Fix 0x8004de40 napaka v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052053"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ce4a7-102">Fix 0x8004de40 napaka v storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="ce4a7-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ce4a7-103">Če prejmete napako 0x8004de40 s storitvijo OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ce4a7-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ce4a7-104">Znova zaženite prizadeti računalnik, medtem ko ste povezani z domeno Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ce4a7-105">Če vnovični zagon ne popravi težave, se Razdruži in znova pridruži napravi iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ce4a7-106">**Opomba**: med izvajanjem teh korakov morate biti v omrežju podjetja.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ce4a7-107">Ne izvajajte teh korakov, ko se ne morete povezati z infrastrukturo podjetja (na primer med potovanjem).</span><span class="sxs-lookup"><span data-stu-id="ce4a7-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ce4a7-108">Odprite visok ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ce4a7-109">Če želite odpreti visok ukazni poziv, kliknite **Start**, z desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ce4a7-110">Vnesite *dsregcmd/Leave* in pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ce4a7-111">Čas celoten, stavek *dsregcmd/združiti* ter časnikarstvo **nastopiti**.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ce4a7-112">Ko končate, zaprite ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ce4a7-113">Znova zaženite računalnik in se prijavite v OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ce4a7-113">Reboot the computer, and log into OneDrive.</span></span>