---
title: Odpravljanje napake v 0x8004de40 v OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745146"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="82d20-102">Odpravljanje napake v 0x8004de40 v OneDrive</span><span class="sxs-lookup"><span data-stu-id="82d20-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="82d20-103">Če prejmete sporočilo o napaki 0x8004de40 z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="82d20-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="82d20-104">Znova zaženite prizadeti računalnik, medtem ko imate vzpostavljeno povezavo z domeno imenika Acitve.</span><span class="sxs-lookup"><span data-stu-id="82d20-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="82d20-105">Če vnovični zagon ne odpravi težave, se obrnite na napravo in se znova pridružite napravi iz storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82d20-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="82d20-106">**Opomba**: med izvajanjem teh korakov morate biti v omrežju podjetja.</span><span class="sxs-lookup"><span data-stu-id="82d20-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="82d20-107">Ne izvajajte teh korakov, če ne morete vzpostaviti povezave z infrastrukturo podjetja (na primer med potovanjem).</span><span class="sxs-lookup"><span data-stu-id="82d20-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="82d20-108">Odprite povišan ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="82d20-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="82d20-109">Če želite odpreti visok ukazni poziv, kliknite **Start**, z desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="82d20-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="82d20-110">Vnesite *dsregcmd/Leave* in pritisnite tipko **Enter**.</span><span class="sxs-lookup"><span data-stu-id="82d20-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="82d20-111">Ko dokončate, vnesite *dsregcmd/JOIN* in pritisnite tipko **Enter**.</span><span class="sxs-lookup"><span data-stu-id="82d20-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="82d20-112">Ko končate, zaprite ukazni poziv.</span><span class="sxs-lookup"><span data-stu-id="82d20-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="82d20-113">Znova zaženite računalnik in se prijavite v OneDrive.</span><span class="sxs-lookup"><span data-stu-id="82d20-113">Reboot the computer, and log into OneDrive.</span></span>