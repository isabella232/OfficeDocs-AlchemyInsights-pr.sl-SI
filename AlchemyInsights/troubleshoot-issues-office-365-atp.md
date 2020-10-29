---
title: Odpravljanje težav z aplikacijo Microsoft Defender za Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801423"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="daac7-102">Odpravljanje težav s sistemom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="daac7-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="daac7-103">Ali ste **opazili zamude pri dostavi e-poštnega sporočila** ?</span><span class="sxs-lookup"><span data-stu-id="daac7-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="daac7-104">Uporabite možnost dinamične dostave za pravilnike o varnih prilogah za ATP.</span><span class="sxs-lookup"><span data-stu-id="daac7-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="daac7-105">S tem se izognete zakasnitvam dostave e-poštnih sporočil, medtem ko ščitite prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="daac7-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="daac7-106">**Ali želite prijaviti lažne pozitivne ali lažne negativne** izraze?</span><span class="sxs-lookup"><span data-stu-id="daac7-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="daac7-107">Uporabite to povezavo, če želite poslati datoteko za analizo: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="daac7-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="daac7-108">**Ali ste vedeli, da lahko omogočite zaščito varne povezave s storitvijo ATP za e-pošto, poslano med osebami v vaši organizaciji** ?</span><span class="sxs-lookup"><span data-stu-id="daac7-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="daac7-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="daac7-109">Follow these steps:</span></span>
    1. <span data-ttu-id="daac7-110">Pojdite na https://protection.office.com in se vpišite.</span><span class="sxs-lookup"><span data-stu-id="daac7-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="daac7-111">Pojdite na **Threat management**  >  **Policy**  >  **varna povezava** pravilnika za upravljanje groženj.</span><span class="sxs-lookup"><span data-stu-id="daac7-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="daac7-112">V razdelku **pravilniki, ki veljajo za določene prejemnike** , uredite (ali dodajte) pravilnik.</span><span class="sxs-lookup"><span data-stu-id="daac7-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="daac7-113">Izberite **uporabi varne povezave do sporočil, poslanih v organizaciji** .</span><span class="sxs-lookup"><span data-stu-id="daac7-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="daac7-114">Shranite pravilnik in počakajte približno 30 minut, da bodo spremembe delovale v podatkovnem središču.</span><span class="sxs-lookup"><span data-stu-id="daac7-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="daac7-115">Če želite pridobiti več pomoči za ATP, glejte [Microsoft Defender za Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="daac7-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>