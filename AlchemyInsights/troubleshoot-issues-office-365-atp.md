---
title: Odpravljanje težav s programom Microsoft Defender za Office 365
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
ms.openlocfilehash: d6170ac52b9af4d2bc6f8822ff2a9b8c1b161ed9
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544774"
---
# <a name="troubleshoot-issues-with-microsoft-defender-for-office-365"></a><span data-ttu-id="ecea0-102">Odpravljanje težav s programom Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="ecea0-102">Troubleshoot issues with Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="ecea0-103">**Ali opazite zakasnitve pri dostavi e-poštnega sporočila?**</span><span class="sxs-lookup"><span data-stu-id="ecea0-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="ecea0-104">Poskusite uporabiti možnost dinamične dostave za pravilnike o prilogah aplikacije Microsoft Defender Office 365 Sef o prilogah.</span><span class="sxs-lookup"><span data-stu-id="ecea0-104">Try using the Dynamic Delivery option for your Microsoft Defender for Office 365 Safe Attachments policies.</span></span> <span data-ttu-id="ecea0-105">Tako boste preprečili zakasnitve dostave e-poštnih sporočil in pri tem zaščitili prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="ecea0-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="ecea0-106">**Ali želite poročati o napačnih pozitivnih ali neresničnih negativnih vrednostih?**</span><span class="sxs-lookup"><span data-stu-id="ecea0-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="ecea0-107">Uporabite [Raziskovalca za pošiljanje.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="ecea0-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>
- <span data-ttu-id="ecea0-108">**Ali ste vedeli, da lahko microsoft Defender za Microsoft Defender** omogočite za zaščito Office 365 Sef za e-pošto, poslano med ljudmi v organizaciji?</span><span class="sxs-lookup"><span data-stu-id="ecea0-108">**Did you know that you can enable Microsoft Defender for Microsoft Defender for Office 365 Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="ecea0-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="ecea0-109">Follow these steps:</span></span>
    1. <span data-ttu-id="ecea0-110">Odprite https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="ecea0-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="ecea0-111">Pojdite na **Povezave**  >  **pravilnika**  >  **za Sef groženj.**</span><span class="sxs-lookup"><span data-stu-id="ecea0-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="ecea0-112">V **razdelku Pravilniki, ki veljajo za določene** prejemnike uredite (ali dodajte) pravilnik.</span><span class="sxs-lookup"><span data-stu-id="ecea0-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="ecea0-113">Izberite **Uporabi varne povezave za sporočila, poslana znotraj organizacije.**</span><span class="sxs-lookup"><span data-stu-id="ecea0-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="ecea0-114">Shranite pravilnik in počakajte do 30 minut, da bodo spremembe veljale.</span><span class="sxs-lookup"><span data-stu-id="ecea0-114">Save your policy, and allow up to 30 minutes for your changes to apply.</span></span>

- <span data-ttu-id="ecea0-115">Če želite več pomoči za aplikacijo Microsoft Defender za Office 365, [glejte Microsoft Defender za Office 365.](/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="ecea0-115">To get more help with Microsoft Defender for Office 365, see [Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/office-365-atp).</span></span>