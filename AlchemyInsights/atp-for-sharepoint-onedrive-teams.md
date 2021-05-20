---
title: Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543593"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="13245-102">Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="13245-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="13245-103">Upoštevajte ta navodila, da omogočite Microsoft Defender Office 365:</span><span class="sxs-lookup"><span data-stu-id="13245-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="13245-104">Pojdite v [https://protection.office.com](https://protection.office.com) račun globalnega skrbnika ali skrbnika za varnost in se vpišite z njim.</span><span class="sxs-lookup"><span data-stu-id="13245-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="13245-105">V levem podoknu za krmarjenje **v razdelku Upravljanje groženj** izberite Pravilnik **Sef** \> **priloge.**</span><span class="sxs-lookup"><span data-stu-id="13245-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="13245-106">Izberite **Vklopi Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams.**</span><span class="sxs-lookup"><span data-stu-id="13245-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="13245-107">[Ustvarite pravilnik o opozorilih o dejavnosti za](/microsoft-365/compliance/create-activity-alerts) prejemanje obvestil, ko zaznamo zlonamerne datoteke.</span><span class="sxs-lookup"><span data-stu-id="13245-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="13245-108">Če želite popolna navodila, glejte [to vklop Sef prilog za SharePoint, OneDrive in Microsoft Teams.](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="13245-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="13245-109">**Opomba:** Microsoft Defender za Office 365 privzeto ne pregleda vseh datotek v storitvi SharePoint Online, OneDrive za podjetja ali Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13245-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="13245-110">Datoteke se asinhrono pregleda s postopkom, ki uporablja dejavnost skupne rabe, dejavnost gosta in signale o grožnjah za prepoznavanje zlonamernih datotek.</span><span class="sxs-lookup"><span data-stu-id="13245-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="13245-111">Če želite več informacij, [glejte Sef Priloge za SharePoint, OneDrive in Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="13245-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
