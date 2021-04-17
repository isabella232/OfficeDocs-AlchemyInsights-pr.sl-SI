---
title: Odpravljanje težav pri včlanitvi naprav s sistemom iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823479"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c8937-102">Odpravljanje težav pri včlanitvi naprav s sistemom iOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c8937-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c8937-103">Preglejte vire spodaj, da odpravite težavo.</span><span class="sxs-lookup"><span data-stu-id="c8937-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c8937-104">Nekatera pogosta sporočila o napakah in koraki za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="c8937-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c8937-105">**Dosežena je bila kapa naprave** Uporabnik ima včlanitev več naprav, kot je omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="c8937-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c8937-106">Preglejte te [dokumente, da odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali spremenite omejitev [naprave.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="c8937-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c8937-107">**Ta storitev ni podprta. Brez pravilnika o včlanitve:** storitev potisnih obvestil Apple Push Notification Service (APNS) je treba konfigurirati ali obnoviti.</span><span class="sxs-lookup"><span data-stu-id="c8937-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c8937-108">Preglejte [ta dokument,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) če želite navodila, kako to naredite.</span><span class="sxs-lookup"><span data-stu-id="c8937-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c8937-109">**Vrsta uporabniške licence Neveljavno ali Uporabniško ime ni prepoznano:** Uporabniku mora biti dodeljena licenca za Intune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="c8937-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c8937-110">Preglejte te dokumente, da dodelite licenco prek: [Skrbniškega središča za Office](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="c8937-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c8937-111">Dodatni viri za odpravljanje težave:</span><span class="sxs-lookup"><span data-stu-id="c8937-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c8937-112">S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani.</span><span class="sxs-lookup"><span data-stu-id="c8937-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c8937-113">Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="c8937-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c8937-114">V dokumentih si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike: Vodnik za odpravljanje težav [in](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [Odpravljanje težav z dokumentom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c8937-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c8937-115">[Preberite, kako včlanite naprave s sistemom iOS v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="c8937-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

