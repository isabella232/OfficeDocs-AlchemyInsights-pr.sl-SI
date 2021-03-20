---
title: Težave s računalniki za upravljanje s storitvijo Microsoft Defender za končne točke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901583"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="c511a-102">Težave s računalniki za upravljanje s storitvijo Microsoft Defender za končne točke</span><span class="sxs-lookup"><span data-stu-id="c511a-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="c511a-103">Morda imate težave s sprejemanjem računalnikov v storitev MDE.</span><span class="sxs-lookup"><span data-stu-id="c511a-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="c511a-104">Če lahko dostopate do računalnika za končnega uporabnika, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="c511a-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="c511a-105">Prenesite najnovejšo predogledno različico orodja za analizo [MDE in](https://aka.ms/betamdeanalyzer) za diagnostiko.</span><span class="sxs-lookup"><span data-stu-id="c511a-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="c511a-106">Z desno tipko **MDEClientAnalyzer.cmd in** »Zaženi kot skrbnik«.</span><span class="sxs-lookup"><span data-stu-id="c511a-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="c511a-107">Upoštevajte vsa predlagana navodila v **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="c511a-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="c511a-108">Če želite več podrobnejših dnevnikov, preglejte ustvarjeno podmapo z imenom **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="c511a-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="c511a-109">Če potrebujete dodatna navodila, se obrnite na podporo za [Microsoft Defender za končno točko](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) navedite nastalo datoteko MDEClientAnalyzerResult.zip za analizo.</span><span class="sxs-lookup"><span data-stu-id="c511a-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
