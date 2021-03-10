---
title: Uporabite osnovne varnostne črte Microsoft InTune, da konfigurirate naprave s sistemom Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696382"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="ab4a7-102">Uporaba osnovnih varnostnih črt za Microsoft InTune za konfiguriranje naprav s sistemom Windows 10</span><span class="sxs-lookup"><span data-stu-id="ab4a7-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="ab4a7-103">InTune varnostne osnovne črte omogočajo zaščito uporabnikov in naprav.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ab4a7-104">Osnovne varnostne črte so nastavitve sistema Windows, ki so bile vnaprej konfigurirane za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporoča ustrezna varnostna ekipa.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ab4a7-105">Z ustvarjanjem profila varnostnega osnovnega načrta v programu InTune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprav.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ab4a7-106">Ko uvedete varnostne osnovne črte v skupine uporabnikov ali naprav, so nastavitve uporabljene v napravah, ki se izvajajo v sistemu Windows 10 ali novejših različicah.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="ab4a7-107">Na primer, če se samodejno varnostno izhodišče Microsoft Mobile Device Management (MDM) (1) omogoči BitLocker za izmenljive pogone, (2) zahteva geslo za sprostitev naprave in (3) onemogoči osnovno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ab4a7-108">Ko privzeta vrednost ne deluje v vašem okolju, lahko prilagodite osnovni načrt, da uporabite nastavitve, ki jih potrebujete.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ab4a7-109">Varnostne osnovne črte omogočajo tudi vzpostavitev varnega poteka dela od konca do konca v programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ab4a7-110">Spodaj so navedene nekatere prednosti te funkcije:</span><span class="sxs-lookup"><span data-stu-id="ab4a7-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="ab4a7-111">V osnovnem načrtu varnosti so na voljo najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ab4a7-112">Ker InTune partnerji z varnostno skupino sistema Windows, ki ustvari osnovne predloge za pravilnike skupine, ta priporočila temeljijo na trdnih navodilih in obširnih izkušnjah.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ab4a7-113">Če ste šele začeli uporabljati InTune in ne veste, kje začeti, vam bodo varnostne osnovne črte pomagale hitro ustvariti in uvesti varen profil.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ab4a7-114">Če trenutno uporabljate pravilnik skupine, je selitev v program za upravljanje precej lažja, saj so te osnovne varnostne črte vgrajene v InTune in vključujejo vrhunske zmogljivosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="ab4a7-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ab4a7-115">Če želite več informacij, glejte [osnovne varnostne črte sistema Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) in [upravljanje mobilnih naprav](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="ab4a7-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>