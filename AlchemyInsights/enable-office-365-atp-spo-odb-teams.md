---
title: Omogočanje sistema Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703442"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c247f-102">Omogoči Office 365 napredno zaščito pred grožnjami za SharePoint online, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c247f-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c247f-103">Pojdite na https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="c247f-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c247f-104">Izberite > **Policy**pravilnik > za **upravljanje groženj\*\*\*\*varne Priloge**.</span><span class="sxs-lookup"><span data-stu-id="c247f-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c247f-105">Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**ter kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="c247f-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c247f-106">Priporočljivo Kot globalni skrbnik ali skrbnik SharePoint online zaženite ukaz [set-spot,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet s parametrom **Disallowinfectedfiledownload** , ki je nastavljen na *True*.</span><span class="sxs-lookup"><span data-stu-id="c247f-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c247f-107">Priporočljivo [Nastavite opozorila](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za odkrite datoteke.</span><span class="sxs-lookup"><span data-stu-id="c247f-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c247f-108">ATP hoteti nČe želite skandirati sleherni posamezen pila v SharePoint online, OneDrive, ali mikroskop skupina.</span><span class="sxs-lookup"><span data-stu-id="c247f-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c247f-109">Datoteke skenirane asinhrono, skozi proces, ki uporablja skupno rabo in gostuje dogodki dejavnosti, skupaj s pametno hevristiko in grožnje signalov za prepoznavanje zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="c247f-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c247f-110">Glej [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams), Poglej.</span><span class="sxs-lookup"><span data-stu-id="c247f-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>