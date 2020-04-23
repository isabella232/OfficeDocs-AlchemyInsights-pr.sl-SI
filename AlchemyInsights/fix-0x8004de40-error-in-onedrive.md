---
title: Fix 0x8004de40 napaka v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716044"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="92e37-102">Fix 0x8004de40 napaka v storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="92e37-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="92e37-103">Če prejmete napako 0x8004de40 s storitvijo OneDrive:</span><span class="sxs-lookup"><span data-stu-id="92e37-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="92e37-104">Znova zaženite prizadeti računalnik, medtem ko ste povezani z domeno Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="92e37-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="92e37-105">Če vnovični zagon ne popravi težave, se Razdruži in znova pridruži napravi iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="92e37-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="92e37-106">**Opomba**: med izvajanjem teh korakov morate biti v omrežju podjetja.</span><span class="sxs-lookup"><span data-stu-id="92e37-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="92e37-107">Ne izvajajte teh korakov, ko se ne morete povezati z infrastrukturo podjetja (na primer med potovanjem).</span><span class="sxs-lookup"><span data-stu-id="92e37-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="92e37-108">Odprite visok ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="92e37-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="92e37-109">Če želite odpreti visok ukazni poziv, kliknite **Start**, z desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="92e37-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="92e37-110">Vnesite *dsregcmd/Leave* in pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="92e37-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="92e37-111">Čas celoten, stavek *dsregcmd/združiti* ter časnikarstvo **nastopiti**.</span><span class="sxs-lookup"><span data-stu-id="92e37-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="92e37-112">Ko končate, zaprite ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="92e37-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="92e37-113">Znova zaženite računalnik in se prijavite v OneDrive.</span><span class="sxs-lookup"><span data-stu-id="92e37-113">Reboot the computer, and log into OneDrive.</span></span>