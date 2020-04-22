---
title: Odpravljanje težav z včlanjanjem naprav Android v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759636"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="5b6f5-102">Odpravljanje težav z včlanjanjem naprav Android v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="5b6f5-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="5b6f5-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="5b6f5-104">Nekatera pogosta vprašanja in koraki reševanja:</span><span class="sxs-lookup"><span data-stu-id="5b6f5-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="5b6f5-105">**Naprava ni šifrirana napaka v portalu podjetja:** Novejše različice Androida, zlasti začenši z v 7.0, zahtevajo geslo za zagon, da zagotovite, da je naprava popolnoma šifrirana.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="5b6f5-106">Pogoste rešitve omogočajo zagonsko kodo ali popolnoma šifriranje naprave.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="5b6f5-107">Če želite več informacij, preglejte [ta dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="5b6f5-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="5b6f5-108">**Naprave ne da se preveri v s storitvijo InTune ali izpis kot "nezdrava" v InTune admin konzolo:** Nekateri Samsung 4,4 in 5,5 naprave morda ne bodo preverili v storitvi.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="5b6f5-109">Obstaja 3 možne rešitve za to vprašanje:</span><span class="sxs-lookup"><span data-stu-id="5b6f5-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="5b6f5-110">Ročno odprite program InTune Company portal, ki bo samodejno inicializiral sinhronizacijo naprave.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="5b6f5-111">Posodobite napravo na Android 6,0 ali novejšo.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="5b6f5-112">Onesposobiti hrust spreten šef s upraven InTune družba portal.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="5b6f5-113">Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za več podrobnosti o teh vprašanjih in resolucijah.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="5b6f5-114">**Uporabniška licenčna vrsta neveljavna** ali **uporabniško ime ni prepoznana napaka:** uporabniku je treba dodeliti licenco InTune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="5b6f5-115">Preglejte te dokumente, če želite dodeliti licenco prek: Officeovega skrbniškega središča ali portala Azure.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="5b6f5-116">Dodatni viri, ki vam pomagajo odpraviti težavo:</span><span class="sxs-lookup"><span data-stu-id="5b6f5-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5b6f5-117">Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5b6f5-118">Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="5b6f5-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="5b6f5-119">Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu.</span><span class="sxs-lookup"><span data-stu-id="5b6f5-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="5b6f5-120">[Naučite se včlaniti naprave Android v Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="5b6f5-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
