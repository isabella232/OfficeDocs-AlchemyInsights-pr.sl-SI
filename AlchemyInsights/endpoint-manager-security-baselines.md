---
title: Endpoint Manager – osnove varnosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440909"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="a4ca2-102">Endpoint Manager – osnove varnosti</span><span class="sxs-lookup"><span data-stu-id="a4ca2-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="a4ca2-103">Osnove varnosti so vnaprej konfigurirane skupine nastavitev sistema Windows, ki vam pomagajo uporabiti varnostne nastavitve, ki jih priporočajo ustrezne varnostne skupine.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="a4ca2-104">Ta izhodišča je mogoče prilagoditi tako, da zagotavljajo samo želene nastavitve in vrednosti.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="a4ca2-105">Za več informacij o varnostnih izhodiščih glejte [Uporaba varnostnih izhodišč za konfiguriranje naprav Windows 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a4ca2-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="a4ca2-106">Trenutno obstajajo osnove za te izdelke:</span><span class="sxs-lookup"><span data-stu-id="a4ca2-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="a4ca2-107">Varnostne nastavitve Windows MDM</span><span class="sxs-lookup"><span data-stu-id="a4ca2-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="a4ca2-108">Microsoft Defender za končno točko</span><span class="sxs-lookup"><span data-stu-id="a4ca2-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="a4ca2-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a4ca2-109">Microsoft Edge</span></span>

<span data-ttu-id="a4ca2-110">Posamezna izhodišča se redno posodabljajo in izdajajo v postopnih različicah.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="a4ca2-111">Vsaka različica doda in odstrani nastavitve iz prejšnje različice, da zagotovi, da osnova ustreza trenutnim navodilom.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="a4ca2-112">Konzola osnov varnosti v programu Endpoint Security omogoča primerjavo različnih različic, tako da so spremembe vidne od različice do različice.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="a4ca2-113">Za napotke o tem, kako najučinkoviteje spremeniti uporabljeno različico osnove, glejte [Upravljanje varnostnih profilov osnovne linije v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="a4ca2-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="a4ca2-114">Po uvedbi osnove varnosti lahko spremljate stanje uvajanja in pregledate nastavitve za vsako napravo posebej.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="a4ca2-115">**Opomba:** Podatki poročanja o napakah za osnove varnosti lahko trajajo do 24 ur, preden se prikažejo od začetne uvedbe do naprave, in do 6 ur za nadaljnje posodobitve.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="a4ca2-116">Najpogostejši vzrok, da se osnovna nastavitev ne uporablja, je zato, ker se ista nastavitev uporablja v drugačnem profilu.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="a4ca2-117">Ta scenarij je mogoče raziskati za določeno napravo tako, da jo izberete v vozlišču Stanje naprave profila osnove varnosti.</span><span class="sxs-lookup"><span data-stu-id="a4ca2-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="a4ca2-118">Če želite izvedeti več, si oglejte [Razreševanje sporov za osnove varnosti](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a4ca2-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>