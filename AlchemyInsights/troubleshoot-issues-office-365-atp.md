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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511128"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="62949-102">Odpravljanje težav z Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="62949-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="62949-103">**Obvestilo zamude pri dostavi e-poštnega sporočila**?</span><span class="sxs-lookup"><span data-stu-id="62949-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="62949-104">Uporabite možnost dinamična dostava za pravilnike o varnih prilogah ATP.</span><span class="sxs-lookup"><span data-stu-id="62949-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="62949-105">S tem se izognete zamudam pri dostavi e-poštnega sporočila, hkrati pa zaščitite prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="62949-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="62949-106">**Ali želite prijaviti lažne pozitivne ali lažne negativce**?</span><span class="sxs-lookup"><span data-stu-id="62949-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="62949-107">Uporabite to povezavo, da pošljete svojo datoteko za analizo:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="62949-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="62949-108">**Ali ste vedeli, da lahko omogočite zaščito ATP Safe Links za e-pošto, poslano med ljudmi v vaši organizaciji**?</span><span class="sxs-lookup"><span data-stu-id="62949-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="62949-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="62949-109">Follow these steps:</span></span>
    1. <span data-ttu-id="62949-110">Pojdi https://protection.office.com in se prijavi.</span><span class="sxs-lookup"><span data-stu-id="62949-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="62949-111">Pojdite na **Threat management**  >  **Policy**  >  **varne povezave**politike obvladovanja groženj.</span><span class="sxs-lookup"><span data-stu-id="62949-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="62949-112">V razdelku **pravilniki, ki veljajo za določene prejemnike**, uredite (ali dodajte) pravilnik.</span><span class="sxs-lookup"><span data-stu-id="62949-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="62949-113">Izberite **uporabi varne povezave do sporočil, poslanih v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="62949-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="62949-114">Shranite pravilnik in pustite približno 30 minut, da spremembe delujejo na poti skozi podatkovno središče.</span><span class="sxs-lookup"><span data-stu-id="62949-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="62949-115">Če želite več pomoči za ATP, glejte [Office 365 napredno zaščito pred grožnjami](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="62949-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>