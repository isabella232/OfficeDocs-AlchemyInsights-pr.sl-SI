---
title: Odpravljanje težav z vpisom naprav Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934792"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="487ad-102">Odpravljanje težav z vpisom naprav Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="487ad-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="487ad-103">Pregledati vire spodaj za zdaj rešiti težavo.</span><span class="sxs-lookup"><span data-stu-id="487ad-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="487ad-104">Neki splošen zmota vest ter odložnost lestev:</span><span class="sxs-lookup"><span data-stu-id="487ad-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="487ad-p101">**Programske opreme ni mogoče namestiti, 0x80cf4017:** Vaš račun potrdilo je poteklo. Drugi ton oktave-travnato gričevje PC odjemalca programski paket v Admin konzoli Intune. Pregled ta dokumentacija za več informacij.</span><span class="sxs-lookup"><span data-stu-id="487ad-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="487ad-108">**Zmota zbornik 0x801c0003:** Napaka se lahko pojavi v naslednjih primerih:</span><span class="sxs-lookup"><span data-stu-id="487ad-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="487ad-p102">Uporabnik ima več naprav, ki so vpisani presega omejitev naprave. Pregled teh dokumentov [odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="487ad-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="487ad-p103">»Uporabniki lahko pridružijo naprave Azure oglas« nastavljen na "brez". Jo nastavite na vse ali izberite Uporabniki. Pregled [ta dokumentacija](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="487ad-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="487ad-p104">Naprava je vpisan že drug uporabnik. Če je temu tako, odstranite napravo iz Azure Intune konzole ali ročno izpisati napravo, preden poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="487ad-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="487ad-p105">Naprava je Windows 10 domov. Samo okno 10 Pro, izobraževanje in podjetja SKUs lahko pridruži Azure storitve Active Directory.</span><span class="sxs-lookup"><span data-stu-id="487ad-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="487ad-118">Dodatna sredstva za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="487ad-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="487ad-p106">Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak. Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="487ad-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="487ad-121">Pregled teh dokumentov seznam pogostih napak, ki preprečujejo včlanitev in resolucije posameznim: [Priročnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="487ad-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="487ad-122">[Naučite se, kako vpisati naprav Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="487ad-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

