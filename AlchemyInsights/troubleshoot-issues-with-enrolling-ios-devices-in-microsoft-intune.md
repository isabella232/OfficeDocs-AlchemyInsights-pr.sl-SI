---
title: Odpravljanje težav z vpisom naprav s sistemom iOS v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708978"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="bec00-102">Odpravljanje težav z vpisom naprav s sistemom iOS v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="bec00-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="bec00-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="bec00-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bec00-104">Nekaj pogostih sporočil o napaki in korakih reševanja:</span><span class="sxs-lookup"><span data-stu-id="bec00-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="bec00-105">**Dosežen je bil pokrovček naprave** Uporabnik ima več naprav, ki so bile včlanjene kot omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="bec00-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bec00-106">Če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), preglejte te dokumente.</span><span class="sxs-lookup"><span data-stu-id="bec00-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="bec00-107">**Ta storitev ni podprta. Št pravilnik o vpisu:** storitev Apple push Service (APNS) mora biti konfigurirana ali obnovljena.</span><span class="sxs-lookup"><span data-stu-id="bec00-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="bec00-108">Oglejte si [ta dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , če želite navodila o tem, kako to naredite.</span><span class="sxs-lookup"><span data-stu-id="bec00-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="bec00-109">**Vrsta uporabniške licence ni veljavna ali pa uporabniško ime ni prepoznano:** Uporabniku je treba dodeliti licenco za InTune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="bec00-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bec00-110">Preglejte te dokumente, če želite dodeliti licenco prek [skrbniškega središča za Office](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="bec00-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="bec00-111">Dodatni viri za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="bec00-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bec00-112">V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu.</span><span class="sxs-lookup"><span data-stu-id="bec00-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bec00-113">Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="bec00-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bec00-114">Preglejte te dokumente za seznam pogostih napak, ki preprečujejo vpis in resolucije za vsako: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav z doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bec00-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="bec00-115">[Naučite se vpisati naprave s sistemom IOS v Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="bec00-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

