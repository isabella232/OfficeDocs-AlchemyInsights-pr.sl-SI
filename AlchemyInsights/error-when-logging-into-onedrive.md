---
title: 0x8004de40 pri zagonu storitve OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813668"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="e3078-102">0x8004de40 pri zagonu storitve OneDrive</span><span class="sxs-lookup"><span data-stu-id="e3078-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="e3078-103">Če se pri prijavi v **OneDrive 0x8004de40** prikaže sporočilo o napaki, znova zaženite računalnik, ko imate vzpostavljeno povezavo s službeno ali šolsko domeno.</span><span class="sxs-lookup"><span data-stu-id="e3078-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="e3078-104">Če po vnovičnem zagonu računalnika prejmete to napako, poskusite to, ko ste povezani s službeno ali šolsko domeno:</span><span class="sxs-lookup"><span data-stu-id="e3078-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="e3078-105">Kliknite Start in v iskalno polje vnesite **cmd** ali **ukazni** poziv, z desno tipko miške kliknite aplikacijo ukaznega poziva in izberite **Zaženi kot skrbnik.**</span><span class="sxs-lookup"><span data-stu-id="e3078-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="e3078-106">Če ste pozvani k vnosu skrbniškega gesla ali potrditvi, vnesite geslo ali kliknite **Dovoli.**</span><span class="sxs-lookup"><span data-stu-id="e3078-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="e3078-107">V okno ukaznega poziva vnesite **dsregcmd /leave**  in počakajte, da se ukaz dokonča.</span><span class="sxs-lookup"><span data-stu-id="e3078-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="e3078-108">Nato vnesite **dsregcmd /join in** počakajte, da se ukaz dokonča.</span><span class="sxs-lookup"><span data-stu-id="e3078-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="e3078-109">Znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="e3078-109">Reboot your computer.</span></span>
