---
title: EndPoint Manager – varnostni osnovni načrt
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421091"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="a0f0d-102">EndPoint Manager – varnostni osnovni načrt</span><span class="sxs-lookup"><span data-stu-id="a0f0d-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="a0f0d-103">Varnostni osnovni načrt so vnaprej konfigurirane skupine nastavitev sistema Windows, s pomočjo teh nastavitev lahko uporabite varnostne nastavitve, ki jih priporočajo ustrezne varnostne skupine.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="a0f0d-104">Te osnovne vrstice je mogoče prilagoditi tako, da zagotavljajo le želene nastavitve in vrednosti.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="a0f0d-105">Če želite več informacij o varnostnih osnovnih črtah, glejte Uporaba varnostnih osnovnih načrta [za konfiguracijo naprav s sistemom Windows 10 v storitvi Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="a0f0d-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="a0f0d-106">Trenutno obstajajo osnovni načrti za te izdelke:</span><span class="sxs-lookup"><span data-stu-id="a0f0d-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="a0f0d-107">Varnostne nastavitve sistema Windows MDM</span><span class="sxs-lookup"><span data-stu-id="a0f0d-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="a0f0d-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="a0f0d-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="a0f0d-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a0f0d-109">Microsoft Edge</span></span>

<span data-ttu-id="a0f0d-110">Vsak osnovni načrt se redno posodablja in izda v postopnih različicah.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="a0f0d-111">Vsaka različica doda in odstrani nastavitve iz prejšnje različice in tako zagotovi, da osnovni načrt izpolnjuje trenutne smernice.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="a0f0d-112">Konzola »Varnostni osnovni osnovni načrt« v varnosti končne točke omogoča, da se različne različice primerjajo tako, da so spremembe vidne iz različice v različico.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="a0f0d-113">Navodila za najučinkovitejšo spremembo, katera različica osnovnega načrta je uvedena, so v članku Upravljanje profilov osnovnega načrta za varnost [v storitvi Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="a0f0d-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="a0f0d-114">Ko uvedete varnostni osnovni načrt, lahko spremljate stanje uvajanja in pregledujete nastavitve na osnovi naprav.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="a0f0d-115">**Opomba:** Podatki poročanja za osnovne vrstice lahko trajajo do 24 ur, da se prikažejo od začetne uvedbe do naprave in do 6 ur za dodatne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="a0f0d-116">Najpogostejši vzrok za neuuporabljena nastavitev osnovnega načrta je, ker se ista nastavitev uporablja v drugem profilu.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="a0f0d-117">Ta scenarij lahko raziščete za določeno napravo tako, da to napravo izberete v vozlišču Stanje naprave v profilu varnostnega osnovnega načrta.</span><span class="sxs-lookup"><span data-stu-id="a0f0d-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="a0f0d-118">Če želite več informacij, [glejte Razreševanje sporov za varnostne osnovne načrte.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="a0f0d-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>