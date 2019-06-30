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
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367305"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="bdde2-102">Odpravljanje težav z vpisom Android naprave v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bdde2-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="bdde2-103">Pregledati vire spodaj za zdaj rešiti težavo.</span><span class="sxs-lookup"><span data-stu-id="bdde2-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bdde2-104">Nekatere pogoste težave in odložnost lestev:</span><span class="sxs-lookup"><span data-stu-id="bdde2-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="bdde2-105">**Naprave niso šifrirani napake v podjetje Portal:** Nove različice Android, zlasti začenši s v7.0, zahtevajo zagonsko kodo, se prepričajte, da naprava je popolnoma šifrirano.</span><span class="sxs-lookup"><span data-stu-id="bdde2-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="bdde2-106">So skupne rešitve omogočajo zagonski pin ali popolnoma šifriranje naprave.</span><span class="sxs-lookup"><span data-stu-id="bdde2-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="bdde2-107">Pregled [tega dokumenta](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="bdde2-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="bdde2-108">**Naprave ne preverite s storitvijo Intune ali prikazati kot "Nezdrava" v admin konzoli Intune:** Nekatere Samsung 4,4 in 5,5 naprave lahko preverja v storitev.</span><span class="sxs-lookup"><span data-stu-id="bdde2-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="bdde2-109">Obstajajo 3 možne rešitve za to težavo:</span><span class="sxs-lookup"><span data-stu-id="bdde2-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="bdde2-110">Ročno odprite app Intune podjetje Portal, ki bo samodejno sproži načrt omedlevičen.</span><span class="sxs-lookup"><span data-stu-id="bdde2-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="bdde2-111">Posodobitev naprave Android 6,0 ali višje.</span><span class="sxs-lookup"><span data-stu-id="bdde2-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="bdde2-112">Onesposobiti Samsung pameten šef od upravljanja Intune podjetje Portal.</span><span class="sxs-lookup"><span data-stu-id="bdde2-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="bdde2-113">Pregled [tega dokumenta](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za več podrobnosti o teh vprašanjih in resolucij.</span><span class="sxs-lookup"><span data-stu-id="bdde2-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="bdde2-114">**Uporabnik dati dovoljenje vrsta neveljavne** ali **uporabniško ime ni prepoznano napaka:** uporabnik potrebuje dodelijo licenco Intune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="bdde2-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bdde2-115">Pregled teh dokumentov dodeliti licenco skozi: Office Admin Center ali Azure portal.</span><span class="sxs-lookup"><span data-stu-id="bdde2-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="bdde2-116">Dodatna sredstva za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="bdde2-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bdde2-117">Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak.</span><span class="sxs-lookup"><span data-stu-id="bdde2-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bdde2-118">Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="bdde2-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bdde2-119">Pregled [tega dokumenta](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo včlanitev in resolucije za vsako.</span><span class="sxs-lookup"><span data-stu-id="bdde2-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="bdde2-120">[Naučite se, kako vpisati Android naprave v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="bdde2-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
