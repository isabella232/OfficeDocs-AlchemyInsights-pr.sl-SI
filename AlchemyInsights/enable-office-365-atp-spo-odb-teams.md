---
title: Omogočanje sistema Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709923"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="7007a-102">Omogočanje napredne zaščite pred grožnjami za Office 365 za SharePoint online, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7007a-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="7007a-103">Pojdite na https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="7007a-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="7007a-104">Izberite **Threat management**  >  **Policy**  >  **varna Priloga**pravilnika za upravljanje groženj.</span><span class="sxs-lookup"><span data-stu-id="7007a-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="7007a-105">Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**in nato kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="7007a-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="7007a-106">Priporočeno Kot globalni skrbnik ali skrbnik SharePoint Onlinea zaženite ukaz» cmdlet « [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** , nastavljenim na *True*.</span><span class="sxs-lookup"><span data-stu-id="7007a-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="7007a-107">Priporočeno [Nastavite opozorila](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za zaznane datoteke.</span><span class="sxs-lookup"><span data-stu-id="7007a-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="7007a-108">ATP bo pregledal vsako posamezno datoteko v storitvi SharePoint online, OneDrive ali Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="7007a-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="7007a-109">Datoteke so asinhrono skenirane, in sicer s postopkom, ki uporablja dogodke skupne rabe in gostujoče dejavnosti, skupaj s pametnimi hevristikami in signali za grožnje, da prepozna zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="7007a-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="7007a-110">Glejte [ATP za SharePoint, OneDrive in Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="7007a-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>