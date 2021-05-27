---
title: Pravila za zmanjšanje površine napadov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676443"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="9b57b-102">Pravila za zmanjšanje površine napadov</span><span class="sxs-lookup"><span data-stu-id="9b57b-102">Attack surface reduction rules</span></span>

<span data-ttu-id="9b57b-103">Izključitev datotek ali map lahko resno zmanjša zaščito, ki jo zagotavljajo pravila za zmanjšanje površine napadov.</span><span class="sxs-lookup"><span data-stu-id="9b57b-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="9b57b-104">Datoteke, ki bi jih blokiralo pravilo, se lahko zaženejo, poročilo ali dogodek pa se ne posname.</span><span class="sxs-lookup"><span data-stu-id="9b57b-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="9b57b-105">Izključitev velja za vsa pravila, ki dovoljujejo izjeme.</span><span class="sxs-lookup"><span data-stu-id="9b57b-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="9b57b-106">Izključitve ASR uporabljajo enako sintakso kot Microsoft Defender Antivirus izključitve.</span><span class="sxs-lookup"><span data-stu-id="9b57b-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="9b57b-107">Če želite več informacij, [glejte Konfiguracija in preverjanje veljavnosti izključitev Microsoft Defender Antivirus pregledih.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9b57b-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="9b57b-108">Če se želite izogniti težavam, preglejte pogoste napake, ki se [jim morate izogniti pri določanju izključitev.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9b57b-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="9b57b-109">Izključitve niso podrte z vsemi pravili ASR.</span><span class="sxs-lookup"><span data-stu-id="9b57b-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="9b57b-110">Če želite preveriti, ali pravilo podpira izključitve, glejte tabelo Pravila za [zmanjšanje števila napadov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="9b57b-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="9b57b-111">Pravila za zmanjšanje površine napadov</span><span class="sxs-lookup"><span data-stu-id="9b57b-111">Attack surface reduction rules</span></span>

<span data-ttu-id="9b57b-112">Površina napadov organizacije vključuje vsa mesta, kjer lahko napadalec ogrozi naprave ali omrežja organizacije.</span><span class="sxs-lookup"><span data-stu-id="9b57b-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="9b57b-113">Zmanjšanje števila napadov pomeni zaščito naprav in omrežja organizacije, pri katerem napadalci ostanejo na manj načinov za izvajanje napadov.</span><span class="sxs-lookup"><span data-stu-id="9b57b-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="9b57b-114">V pomoč so lahko pravila za zmanjšanje površine napadov v programu Microsoft Defender za končno točko.</span><span class="sxs-lookup"><span data-stu-id="9b57b-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="9b57b-115">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="9b57b-115">For more information, see:</span></span>

- [<span data-ttu-id="9b57b-116">Guid pravila »Preslikaj kot pravilo ASR za ime</span><span class="sxs-lookup"><span data-stu-id="9b57b-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="9b57b-117">Zahteve pravil ASR:</span><span class="sxs-lookup"><span data-stu-id="9b57b-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="9b57b-118">Windows 10 Pro, različica 1709 ali novejša</span><span class="sxs-lookup"><span data-stu-id="9b57b-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="9b57b-119">Windows 10 Enterprise, različica 1709 ali novejša</span><span class="sxs-lookup"><span data-stu-id="9b57b-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="9b57b-120">Windows Strežnik, različica 1803 (polletni kanal) ali novejša različica</span><span class="sxs-lookup"><span data-stu-id="9b57b-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="9b57b-121">Določite pravilno izključitev, ki jo želite uporabiti</span><span class="sxs-lookup"><span data-stu-id="9b57b-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="9b57b-122">Poiščite ID dogodka 1121 ali 1122 v Microsoftovem Windows-Windows Defender/dnevniku delovanja.</span><span class="sxs-lookup"><span data-stu-id="9b57b-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="9b57b-123">Ocenite scenarij blokiranja in kontekst ter potrdite, da je treba ta scenarij odblokiran.</span><span class="sxs-lookup"><span data-stu-id="9b57b-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="9b57b-124">Preberite vrednost Path (Pot) v podrobnostih dogodka, ki je vrednost, ki določa izključitev.</span><span class="sxs-lookup"><span data-stu-id="9b57b-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="9b57b-125">Izključitev naj bo čim bolj stroga.</span><span class="sxs-lookup"><span data-stu-id="9b57b-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="9b57b-126">Po potrebi uporabite nadomestni znak (nadomestite na primer »Uporabnik spremenljivka«).</span><span class="sxs-lookup"><span data-stu-id="9b57b-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="9b57b-127">Uporabite izključitev glede na potrebe uvajanja.</span><span class="sxs-lookup"><span data-stu-id="9b57b-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="9b57b-128">Če želite več informacij, [glejte Prilagajanje pravil za zmanjšanje površine napadov.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="9b57b-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="9b57b-129">Izključitev ni v skladu s</span><span class="sxs-lookup"><span data-stu-id="9b57b-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="9b57b-130">Določite, ali pravilo podpira izključitve.</span><span class="sxs-lookup"><span data-stu-id="9b57b-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="9b57b-131">Če želite več informacij, glejte [Pravila za zmanjšanje števila napadov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="9b57b-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="9b57b-132">Preglejte uporabljene izjeme in preverite, ali so v podatkih o dogodku morda tipkarske napake ali nadomestni znaki, ki se narobe tolmačijo.</span><span class="sxs-lookup"><span data-stu-id="9b57b-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="9b57b-133">Če želite več informacij, glejte [Podprte vrste izključitev](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="9b57b-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="9b57b-134">če je vpliv pravila prenizka, premislite o premiku pravila (nazaj) v način nadzora, da izvedete dodatno preverjanje veljavnosti.</span><span class="sxs-lookup"><span data-stu-id="9b57b-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="9b57b-135">Če želite več informacij, [glejte Preskus delovanja programa Microsoft Defender for Endpoint v načinu nadzora.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="9b57b-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="9b57b-136">S tem ukazom zberite podatke podpore, da odprete primer podpore:</span><span class="sxs-lookup"><span data-stu-id="9b57b-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="9b57b-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="9b57b-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="9b57b-138">Če želite več informacij, glejte [Težave s računalniki za upravljanje s programom Microsoft Defender za končne točke.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="9b57b-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
