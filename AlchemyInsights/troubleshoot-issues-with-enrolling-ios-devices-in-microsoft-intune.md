---
title: Odpravljanje težav z včlanjanjem naprav iOS v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736174"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2ce79-102">Odpravljanje težav z včlanjanjem naprav iOS v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="2ce79-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2ce79-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="2ce79-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2ce79-104">Nekatera pogosta sporočila o napakah in koraki reševanja:</span><span class="sxs-lookup"><span data-stu-id="2ce79-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2ce79-105">**Naprava SKP dosežena** Uporabnik ima več naprav, vpisanih kot omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="2ce79-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2ce79-106">Preglejte te dokumente, če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2ce79-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2ce79-107">**Ta storitev ni podprta. Št vpis politika:** Apple push obvestilo Service (APNS) je treba konfigurirati ali obnoviti.</span><span class="sxs-lookup"><span data-stu-id="2ce79-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2ce79-108">Preglejte [ta dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , če želite navodila za to.</span><span class="sxs-lookup"><span data-stu-id="2ce79-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2ce79-109">**Uporabniška licenčna vrsta neveljavna ali uporabniško ime ni bilo prepoznano:** Uporabniku je treba dodeliti licenco InTune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="2ce79-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2ce79-110">Preglejte te dokumente, če želite dodeliti licenco prek: [Officeovega skrbniškega središča](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2ce79-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2ce79-111">Dodatni viri, ki vam pomagajo odpraviti težavo:</span><span class="sxs-lookup"><span data-stu-id="2ce79-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2ce79-112">Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve.</span><span class="sxs-lookup"><span data-stu-id="2ce79-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2ce79-113">Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="2ce79-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2ce79-114">Preglejte te dokumente za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav z zdravnikom](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2ce79-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2ce79-115">[Naučite se včlaniti naprave IOS v Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2ce79-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

