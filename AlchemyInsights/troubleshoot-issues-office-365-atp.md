---
title: Odpravljanje težav s funkcijo Office 365 napredno zaščito pred grožnjami (ATP)
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
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766761"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="64064-102">Odpravljanje težav z Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="64064-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="64064-103">**Obvestilo zamude pri dostavi e-poštnega sporočila**?</span><span class="sxs-lookup"><span data-stu-id="64064-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="64064-104">Uporabite možnost dinamična dostava za pravilnike o varnih prilogah ATP.</span><span class="sxs-lookup"><span data-stu-id="64064-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="64064-105">S tem se izognete zamudam pri dostavi e-poštnega sporočila, hkrati pa zaščitite prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="64064-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="64064-106">**Ali želite prijaviti lažne pozitivne ali lažne negativce**?</span><span class="sxs-lookup"><span data-stu-id="64064-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="64064-107">Uporabite to povezavo, da pošljete svojo datoteko za analizo:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="64064-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="64064-108">**Ali ste vedeli, da lahko omogočite zaščito ATP Safe Links za e-pošto, poslano med ljudmi v vaši organizaciji**?</span><span class="sxs-lookup"><span data-stu-id="64064-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="64064-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="64064-109">Follow these steps:</span></span>
    1. <span data-ttu-id="64064-110">https://protection.office.comPojdi in se prijavi.</span><span class="sxs-lookup"><span data-stu-id="64064-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="64064-111">Pojdite na**varne povezave** > **politike** >  **obvladovanja groženj**.</span><span class="sxs-lookup"><span data-stu-id="64064-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="64064-112">V razdelku **pravilniki, ki veljajo za določene prejemnike**, uredite (ali dodajte) pravilnik.</span><span class="sxs-lookup"><span data-stu-id="64064-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="64064-113">Izberite **uporabi varne povezave do sporočil, poslanih v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="64064-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="64064-114">Shranite pravilnik in pustite približno 30 minut, da spremembe delujejo na poti skozi podatkovno središče.</span><span class="sxs-lookup"><span data-stu-id="64064-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="64064-115">Če želite več pomoči za ATP, glejte [Office 365 napredno zaščito pred grožnjami](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="64064-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>