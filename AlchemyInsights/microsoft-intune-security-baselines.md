---
title: Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794130"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="1b8ae-102">Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave</span><span class="sxs-lookup"><span data-stu-id="1b8ae-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="1b8ae-103">Osnovni osnovni osnovni stroški varnosti za Intune ščitijo uporabnike in naprave.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1b8ae-104">Varnostni osnovni osnovni Windows vnaprej konfigurirane skupine, ki se uporabljajo za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporočajo ustrezne varnostne skupine.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1b8ae-105">Z ustvarjanjem profila varnostnega osnovnega načrta v programu Intune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprave.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1b8ae-106">Ko uvedete varnostne osnovne vrstice za skupine uporabnikov ali naprav, so nastavitve uporabljene za naprave, ki se izvajajo v Windows 10 ali novejših različicah.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="1b8ae-107">Na primer, varnostna osnovna črta upravljanja Microsoftovih mobilnih naprav (MDM) samodejno omogoči BitLocker za izmenljive pogone, zahteva geslo za odklepanje naprave in onemogoči osnovno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="1b8ae-108">Če privzeta vrednost ne deluje v vašem okolju, lahko osnovni načrt prilagodite tako, da uporabi nastavitve, ki jih potrebujete.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1b8ae-109">Z varnostnimi osnovnimi črtami lahko tudi vzpostavite varen potek dela v Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1b8ae-110">Osnovni načrt varnosti vključuje najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1b8ae-111">Intune v sodelovanju z varnostno Windows, ki ustvari osnovne vrstice za pravilnike skupine, zato ta priporočila temeljijo na zanesljivih navodilih in obsežni izkušnji.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="1b8ae-112">Če še ne veste, kje začeti Intune, in ne veste, kje začeti, vam varnostni osnovni načrt pomaga hitro ustvariti in uvesti varen profil.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="1b8ae-113">Če trenutno uporabljate pravilnik skupine, je selitev v Intune za namene upravljanja veliko preprostejša z varnostnimi osnovnimi črtami, ker so vgrajeni v Intune in vključujejo vrhunske zmogljivosti upravljanja.</span><span class="sxs-lookup"><span data-stu-id="1b8ae-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="1b8ae-114">Če želite več informacij, [Windows varnostne osnovne vrstice](/windows/security/threat-protection/windows-security-baselines) [in Upravljanje mobilnih naprav.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="1b8ae-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

