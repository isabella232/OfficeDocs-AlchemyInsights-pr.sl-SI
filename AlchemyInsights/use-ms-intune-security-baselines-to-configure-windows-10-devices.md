---
title: Uporabite Microsoft InTune varnostne osnovne črte, da konfigurirate naprave s sistemom Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573788"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="ac085-102">Uporabite Microsoft InTune varnostne osnovne črte, da konfigurirate naprave s sistemom Windows 10</span><span class="sxs-lookup"><span data-stu-id="ac085-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="ac085-103">InTune varnostne osnovne črte omogočajo zaščito uporabnikov in naprav.</span><span class="sxs-lookup"><span data-stu-id="ac085-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ac085-104">Osnovne varnostne črte so nastavitve sistema Windows, ki so bile vnaprej konfigurirane za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporoča ustrezna varnostna ekipa.</span><span class="sxs-lookup"><span data-stu-id="ac085-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ac085-105">Z ustvarjanjem profila varnostnega osnovnega načrta v programu InTune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprav.</span><span class="sxs-lookup"><span data-stu-id="ac085-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ac085-106">Ko uvedete varnostne osnovne črte v skupine uporabnikov ali naprav, so nastavitve uporabljene v napravah, ki se izvajajo v sistemu Windows 10 ali novejši različici.</span><span class="sxs-lookup"><span data-stu-id="ac085-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="ac085-107">Na primer, MDM Security Basicove vrstice samodejno (1) omogoči BitLocker za izmenljive pogone, (2) zahteva geslo za sprostitev naprave in (3) onemogoči osnovno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="ac085-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ac085-108">Ko privzeta vrednost ne deluje v vašem okolju, prilagodite osnovni načrt, da uporabite nastavitve, ki jih potrebujete.</span><span class="sxs-lookup"><span data-stu-id="ac085-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ac085-109">Varnostne osnovne črte omogočajo tudi vzpostavitev varnega poteka dela od konca do konca v programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ac085-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ac085-110">Spodaj so navedene nekatere prednosti:</span><span class="sxs-lookup"><span data-stu-id="ac085-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="ac085-111">V osnovnem načrtu varnosti so na voljo najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost.</span><span class="sxs-lookup"><span data-stu-id="ac085-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ac085-112">Ker InTune partnerji z varnostno skupino sistema Windows, ki ustvari osnovne predloge za pravilnike skupine, ta priporočila temeljijo na trdnih navodilih in obširnih izkušnjah.</span><span class="sxs-lookup"><span data-stu-id="ac085-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ac085-113">Če ste šele začeli uporabljati InTune in ne veste, kje začeti, vam bodo varnostne osnovne črte pomagale hitro ustvariti in uvesti varen profil.</span><span class="sxs-lookup"><span data-stu-id="ac085-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ac085-114">Če trenutno uporabljate pravilnik skupine, je selitev v InTune za upravljanje precej lažja z osnovnimi varnostnimi črtami, ker so vgrajene v InTune in vključujejo vrhunske zmogljivosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="ac085-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ac085-115">Če želite izvedeti več, glejte [osnovne varnostne črte sistema Windows](https://go.microsoft.com/fwlink/?linkid=2141503) in [upravljanje mobilnih naprav](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="ac085-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>