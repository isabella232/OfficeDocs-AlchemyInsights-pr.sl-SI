---
title: Usposobiti Office 365 ATP za SharePoint, OneDrive in Microsoft ekipe
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403049"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="f113c-102">Usposobiti Office 365 napreden grožnja varstvo za SharePoint Online, OneDrive in Microsoft ekipe</span><span class="sxs-lookup"><span data-stu-id="f113c-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="f113c-103">Pojdi na https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="f113c-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="f113c-104">Izberite **upravljanje nevarnosti** > **politika** > **Varno Priloge**.</span><span class="sxs-lookup"><span data-stu-id="f113c-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="f113c-105">Izberite **Vklop ATP za SharePoint, OneDrive, in Microsoft ekipe**, in nato kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="f113c-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="f113c-106">(Priporočeno) Kot globalni skrbnik ali skrbnik za SharePoint Online, zaženite ukaz »cmdlet« [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parameter **DisallowInfectedFileDownload** nastavite na *true*.</span><span class="sxs-lookup"><span data-stu-id="f113c-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="f113c-107">(Priporočeno) [Nastavite opozorila](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za odkrite datoteke.</span><span class="sxs-lookup"><span data-stu-id="f113c-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="f113c-108">ATP bo skeniranje nto vsak eno datoteko v SharePoint Online, OneDrive, ali Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f113c-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="f113c-109">Datoteke so pregledane asinhrono, skozi proces, ki uporablja skupno rabo in gost dejavnost dogodkov, spreten tolči in signale nevarnost ugotoviti zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="f113c-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="f113c-110">Glej [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="f113c-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>