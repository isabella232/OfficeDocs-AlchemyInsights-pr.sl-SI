---
title: ATP za SharePoint, OneDrive in Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715577"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="87446-102">ATP za SharePoint, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="87446-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="87446-103">Upoštevajte ta navodila, da omogočite dodatno zaščito pred grožnjami:</span><span class="sxs-lookup"><span data-stu-id="87446-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="87446-104">Pojdite na [https://protection.office.com](https://protection.office.com) in se vpišite z računom globalnega skrbnika ali varnostnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="87446-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="87446-105">V levem podoknu za krmarjenje pod možnostjo» **upravljanje grožnje**«izberite» **Policy** \> **varne Priloge**pravilnika «.</span><span class="sxs-lookup"><span data-stu-id="87446-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="87446-106">Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="87446-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="87446-107">[Ustvarjanje pravilnika o opozorilih dejavnosti](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) za prejemanje obvestil, ko zaznamo zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="87446-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="87446-108">Če želite dokončati navodila, si oglejte to [temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="87446-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="87446-109">**Opomba**: v programu SharePoint online, OneDrive za podjetja ali Microsoft Teams ni mogoče skenirati posameznih datotek.</span><span class="sxs-lookup"><span data-stu-id="87446-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="87446-110">Datoteke so asinhrono skenirane s procesom, ki uporablja dejavnost skupne rabe, dejavnosti gosta in signala za grožnje, da prepozna zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="87446-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="87446-111">Če želite več informacij, glejte to [temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="87446-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
