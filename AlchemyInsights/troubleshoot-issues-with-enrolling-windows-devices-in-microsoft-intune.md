---
title: Odpravljanje težav z vpisom naprav sistema Windows v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658894"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f4e20-102">Odpravljanje težav z vpisom naprav sistema Windows v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="f4e20-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f4e20-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="f4e20-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f4e20-104">Nekaj pogostih sporočil o napaki in korakih reševanja:</span><span class="sxs-lookup"><span data-stu-id="f4e20-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f4e20-105">**Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo vašega računa je poteklo.</span><span class="sxs-lookup"><span data-stu-id="f4e20-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="f4e20-106">Znova Prenesite programski paket odjemalca za računalnik s sistemom Windows v konzoli za InTune.</span><span class="sxs-lookup"><span data-stu-id="f4e20-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="f4e20-107">Če želite več informacij, si oglejte to dokumentacijo.</span><span class="sxs-lookup"><span data-stu-id="f4e20-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="f4e20-108">**Koda napake 0x801c0003:** Do napake lahko pride v teh primerih:</span><span class="sxs-lookup"><span data-stu-id="f4e20-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="f4e20-109">Uporabnik ima več naprav, ki so bile včlanjene kot omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="f4e20-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f4e20-110">Če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), preglejte te dokumente.</span><span class="sxs-lookup"><span data-stu-id="f4e20-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="f4e20-111">» Uporabniki lahko priključijo naprave na Azure AD «je nastavljena na» brez «.</span><span class="sxs-lookup"><span data-stu-id="f4e20-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="f4e20-112">Nastavite vse ali izberite uporabnike.</span><span class="sxs-lookup"><span data-stu-id="f4e20-112">Set it to all or select users.</span></span> <span data-ttu-id="f4e20-113">Če želite več informacij, si oglejte [to dokumentacijo](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="f4e20-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="f4e20-114">Napravo je že vpisal drug uporabnik.</span><span class="sxs-lookup"><span data-stu-id="f4e20-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="f4e20-115">Če je to res, odstranite napravo iz konzole Azure InTune ali pa jo ročno odpeljite, preden poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="f4e20-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="f4e20-116">Naprava je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="f4e20-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="f4e20-117">V storitvi Azure Active Directory se lahko pridružite le Windows 10 Pro, izobraževanje in podjetje SKUs.</span><span class="sxs-lookup"><span data-stu-id="f4e20-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="f4e20-118">Dodatni viri za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="f4e20-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="f4e20-119">V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu.</span><span class="sxs-lookup"><span data-stu-id="f4e20-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f4e20-120">Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="f4e20-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="f4e20-121">Preglejte te dokumente za seznam pogostih napak, ki preprečujejo vpis in resolucije za vsako: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav z doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f4e20-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="f4e20-122">[Naučite se vpisati naprave s sistemom Windows v Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f4e20-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
