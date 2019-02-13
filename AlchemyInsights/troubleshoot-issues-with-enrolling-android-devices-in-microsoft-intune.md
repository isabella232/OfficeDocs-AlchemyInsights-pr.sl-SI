---
title: Odpravljanje težav z vpisom Android naprave v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939364"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ec92c-102">Odpravljanje težav z vpisom Android naprave v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ec92c-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ec92c-103">Pregledati vire spodaj za zdaj rešiti težavo.</span><span class="sxs-lookup"><span data-stu-id="ec92c-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ec92c-104">Nekatere pogoste težave in odložnost lestev:</span><span class="sxs-lookup"><span data-stu-id="ec92c-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ec92c-p101">**Naprave niso šifrirani napake v podjetje Portal:** Nove različice Android, zlasti začenši s v7.0, zahtevajo zagonsko kodo, se prepričajte, da naprava je popolnoma šifrirano. So skupne rešitve omogočajo zagonski pin ali popolnoma šifriranje naprave. Pregled [tega dokumenta](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="ec92c-p102">**Naprave ne preverite s storitvijo Intune ali prikazati kot "Nezdrava" v admin konzoli Intune:** Nekatere Samsung 4,4 in 5,5 naprave lahko preverja v storitev. Obstajajo 3 možne rešitve za to težavo:</span><span class="sxs-lookup"><span data-stu-id="ec92c-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="ec92c-110">Ročno odprite app Intune podjetje Portal, ki bo samodejno sproži načrt omedlevičen.</span><span class="sxs-lookup"><span data-stu-id="ec92c-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="ec92c-111">Posodobitev naprave Android 6,0 ali višje.</span><span class="sxs-lookup"><span data-stu-id="ec92c-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="ec92c-p103">Onesposobiti Samsung pameten šef od upravljanja Intune podjetje Portal. Pregled [tega dokumenta](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za več podrobnosti o teh vprašanjih in resolucij.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="ec92c-p104">**Uporabnik dati dovoljenje vrsta neveljavne** ali **uporabniško ime ni prepoznano napaka:** uporabnik potrebuje dodelijo licenco Intune ali EMS. Pregled teh dokumentov dodeliti licenco skozi: Office Admin Center ali Azure portal.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="ec92c-116">Dodatna sredstva za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="ec92c-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ec92c-p105">Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak. Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ec92c-119">Pregled [tega dokumenta](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo včlanitev in resolucije za vsako.</span><span class="sxs-lookup"><span data-stu-id="ec92c-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="ec92c-120">[Naučite se, kako vpisati Android naprave v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ec92c-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

