---
title: Odpravljanje težav z vpisom iOS naprave v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507019"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="69a60-102">Odpravljanje težav z vpisom iOS naprave v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="69a60-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="69a60-103">Pregledati vire spodaj za zdaj rešiti težavo.</span><span class="sxs-lookup"><span data-stu-id="69a60-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="69a60-104">Neki splošen zmota vest ter odložnost lestev:</span><span class="sxs-lookup"><span data-stu-id="69a60-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="69a60-105">**Naprava SKP dosegel** Uporabnik ima več naprav, ki so vpisani presega omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="69a60-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="69a60-106">Pregled teh dokumentov [odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="69a60-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="69a60-107">**Ta storitev ni podprta. Noben vpis pravilnik:** Apple Push obvestila storitev (APNS) mora biti nastavljen ali podaljšati.</span><span class="sxs-lookup"><span data-stu-id="69a60-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="69a60-108">Pregled [tega dokumenta](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za navodila o tem, kako to storiti.</span><span class="sxs-lookup"><span data-stu-id="69a60-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="69a60-109">**Uporabnik dati dovoljenje vrsta neveljavne ali uporabniško ime ni prepoznano:** Uporabnik potrebuje, dodelijo licenco Intune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="69a60-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="69a60-110">Pregled teh dokumentov dodeliti licenco skozi: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ali [sinje portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="69a60-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="69a60-111">Dodatna sredstva za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="69a60-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="69a60-112">Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak.</span><span class="sxs-lookup"><span data-stu-id="69a60-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="69a60-113">Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="69a60-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="69a60-114">Pregled teh dokumentov seznam pogostih napak, ki preprečujejo včlanitev in resolucije posameznim: [Priročnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="69a60-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="69a60-115">[Naučite se, kako vpisati iOS naprave v Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="69a60-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

