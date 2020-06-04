---
title: Odpravljanje težav z včlanjanjem v naprave s sistemom Windows v programu Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665848"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="3f391-102">Odpravljanje težav z včlanjanjem v naprave s sistemom Windows v programu Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="3f391-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="3f391-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="3f391-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3f391-104">Nekatera pogosta sporočila o napakah in koraki reševanja:</span><span class="sxs-lookup"><span data-stu-id="3f391-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="3f391-105">**Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo o računu je poteklo.</span><span class="sxs-lookup"><span data-stu-id="3f391-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="3f391-106">Re-Download PC Client paket programske opreme v InTune admin Console.</span><span class="sxs-lookup"><span data-stu-id="3f391-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="3f391-107">Za več informacij preglejte to dokumentacijo.</span><span class="sxs-lookup"><span data-stu-id="3f391-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="3f391-108">**Koda napake 0x801c0003:** Napaka se lahko pojavi v naslednjih scenarijih:</span><span class="sxs-lookup"><span data-stu-id="3f391-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="3f391-109">Uporabnik ima več naprav, vpisanih kot omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="3f391-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3f391-110">Preglejte te dokumente, če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3f391-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="3f391-111">"Uporabnik maj združiti načrt v Azure AD" je število enakih oseb v "nič".</span><span class="sxs-lookup"><span data-stu-id="3f391-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="3f391-112">Nastavite jo na vse ali izberite uporabnike.</span><span class="sxs-lookup"><span data-stu-id="3f391-112">Set it to all or select users.</span></span> <span data-ttu-id="3f391-113">Če želite več informacij, preglejte [to dokumentacijo](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="3f391-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="3f391-114">Napravo je že vpisal drug uporabnik.</span><span class="sxs-lookup"><span data-stu-id="3f391-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="3f391-115">V tem primeru odstranite napravo iz konzole Azure InTune ali ročno izvlecite napravo, preden znova poskušate.</span><span class="sxs-lookup"><span data-stu-id="3f391-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="3f391-116">Naprava je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="3f391-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="3f391-117">V Azure Active Directory se lahko pridružijo samo Windows 10 Pro, izobraževanje in Enterprise SKUs.</span><span class="sxs-lookup"><span data-stu-id="3f391-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="3f391-118">Dodatni viri, ki vam pomagajo odpraviti težavo:</span><span class="sxs-lookup"><span data-stu-id="3f391-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="3f391-119">Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve.</span><span class="sxs-lookup"><span data-stu-id="3f391-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3f391-120">Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="3f391-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="3f391-121">Preglejte te dokumente za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav z zdravnikom](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3f391-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="3f391-122">[Naučite se včlaniti naprave Windows v Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="3f391-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
