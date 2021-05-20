---
title: Omogočanje Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543944"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="6fd73-102">Omogočite Microsoft Defender za Office 365 za SharePoint Online, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6fd73-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="6fd73-103">Pojdite v https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="6fd73-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="6fd73-104">Izberite **Pravilnik za upravljanje**  >  **groženj** Sef  >  **priloge.**</span><span class="sxs-lookup"><span data-stu-id="6fd73-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="6fd73-105">Izberite **Vklopi Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams** in nato kliknite **Shrani.**</span><span class="sxs-lookup"><span data-stu-id="6fd73-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="6fd73-106">(Priporočeno) Kot globalni skrbnik ali skrbnik storitve SharePoint Online zaženite ukaz »cmdlet« [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload,** nastavljenim na *true.*</span><span class="sxs-lookup"><span data-stu-id="6fd73-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="6fd73-107">(Priporočeno) [Nastavite opozorila](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za zaznane datoteke.</span><span class="sxs-lookup"><span data-stu-id="6fd73-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="6fd73-108">Microsoft Defender for Office 365 ne bo optično preglejl vseh datotek v storitvi SharePoint Online, OneDrive ali Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6fd73-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="6fd73-109">Datoteke so pregledane asinhrono, s postopkom, ki uporablja dogodke skupne rabe in dejavnosti gostov, skupaj s pametnimi heuristično in signali groženj za identifikacijo zlonamernih datotek.</span><span class="sxs-lookup"><span data-stu-id="6fd73-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="6fd73-110">Glejte [Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="6fd73-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>