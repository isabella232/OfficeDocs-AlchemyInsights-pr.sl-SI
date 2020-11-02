---
title: 0x8004de40 Napaka pri zagonu OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823118"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="bec22-102">0x8004de40 Napaka pri zagonu OneDrive</span><span class="sxs-lookup"><span data-stu-id="bec22-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="bec22-103">Če prejmete sporočilo o napaki **0x8004de40** pri prijavi v OneDrive, znova zaženite računalnik, medtem ko imate vzpostavljeno povezavo s službenim ali šolskim domeno.</span><span class="sxs-lookup"><span data-stu-id="bec22-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="bec22-104">Če se po vnovičnem zagonu prikaže to sporočilo o napaki, poskusite to, medtem ko imate vzpostavljeno povezavo s službenim ali šolskim domeno:</span><span class="sxs-lookup"><span data-stu-id="bec22-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="bec22-105">Kliknite Start in vnesite **cmd** ali **ukazni poziv**  v iskalno polje, z desno tipko miške kliknite aplikacijo ukazni poziv, nato pa izberite  **Zaženi kot skrbnik** .</span><span class="sxs-lookup"><span data-stu-id="bec22-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="bec22-106">Če ste pozvani k skrbniškemu geslu ali potrditvi, vnesite geslo ali kliknite **Dovoli** .</span><span class="sxs-lookup"><span data-stu-id="bec22-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="bec22-107">V okno ukazni poziv vnesite **dsregcmd/Leave**  in počakajte, da se ukaz dokonča.</span><span class="sxs-lookup"><span data-stu-id="bec22-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="bec22-108">Nato vnesite **dsregcmd/JOIN** in počakajte, da se ukaz dokonča.</span><span class="sxs-lookup"><span data-stu-id="bec22-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="bec22-109">Znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="bec22-109">Reboot your computer.</span></span>
