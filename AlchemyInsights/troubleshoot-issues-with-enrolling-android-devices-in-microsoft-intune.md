---
title: Odpravljanje težav z vpisom naprav s sistemom Android v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689970"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ab5d9-102">Odpravljanje težav z vpisom naprav s sistemom Android v Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="ab5d9-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ab5d9-103">Preglejte spodaj navedene vire, da odpravite težavo zdaj.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ab5d9-104">Nekaj pogostih težav in korakov reševanja:</span><span class="sxs-lookup"><span data-stu-id="ab5d9-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ab5d9-105">**Napaka v napravi ni šifrirana v portalu podjetja:** Novejše različice sistema Android, še posebej za začetek z v 7.0, zahtevajo zagonsko kodo, da se prepričate, da je naprava popolnoma šifrirana.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ab5d9-106">Pogoste rešitve so, da omogočite zagonski PIN ali popolnoma šifrirate napravo.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ab5d9-107">Če želite več informacij, preglejte [ta dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="ab5d9-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ab5d9-108">**Naprave se ne morejo sprostiti s storitvijo InTune ali prikazati kot» nezdrava «v konzoli za InTune:** Nekatere naprave Samsung 4,4 in 5,5 se morda ne bodo preverjale v storitvi.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ab5d9-109">V tej težavi so na voljo 3 možne rešitve:</span><span class="sxs-lookup"><span data-stu-id="ab5d9-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ab5d9-110">Ročno odprite program InTune Company portal, ki samodejno sproži sinhronizacijo naprave.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ab5d9-111">Posodobite napravo s sistemom Android 6,0 ali novejšo različico.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ab5d9-112">Onemogočanje programa Samsung Smart Manager za upravljanje portala za InTune.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ab5d9-113">Če želite več podrobnosti o teh težavah in resolucijah, preglejte [ta dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .</span><span class="sxs-lookup"><span data-stu-id="ab5d9-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ab5d9-114">**Vrsta uporabniških licenc neveljavna** ali pa **uporabniško ime ni prepoznana napaka:** uporabnik mora dodeliti licenco za InTune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ab5d9-115">Preglejte te dokumente, če želite dodeliti licenco prek skrbniškega središča za Office ali portala Azure.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ab5d9-116">Dodatni viri za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="ab5d9-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ab5d9-117">V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ab5d9-118">Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="ab5d9-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ab5d9-119">Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo vpis in resolucije.</span><span class="sxs-lookup"><span data-stu-id="ab5d9-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ab5d9-120">[Naučite se vpisati naprave s sistemom Android v Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ab5d9-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
