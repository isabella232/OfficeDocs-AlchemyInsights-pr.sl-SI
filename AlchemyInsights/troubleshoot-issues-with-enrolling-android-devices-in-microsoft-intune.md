---
title: Odpravljanje težav pri včlanitvi naprav s sistemom Android v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830958"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="b9d4e-102">Odpravljanje težav pri včlanitvi naprav s sistemom Android v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b9d4e-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="b9d4e-103">Preglejte vire spodaj, da odpravite težavo.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b9d4e-104">Nekatere pogoste težave in koraki za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="b9d4e-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="b9d4e-105">**Napaka, da naprava ni šifrirana v Company Portal:** Novejše različice sistema Android, ki se začnejo s sistemom v7.0, zahtevajo zagonsko geslo, s tem pa se prepričate, da je naprava v celoti šifrirana.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="b9d4e-106">Običajne rešitve so, da omogočite pripenjanje pin-a ob zagonu ali v celoti šifrirate napravo.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="b9d4e-107">Preglejte [ta dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) če želite več informacij.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="b9d4e-108">Naprave se ne prijavijo v storitvi Intune ali pa so v skrbniški konzoli **za Intune prikazane kot »neprimerne«:** Nekateri napravi Samsung 4.4 in 5.5 se morda ne prijavita v storitev.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="b9d4e-109">Za to težavo so na voljo 3 rešitve:</span><span class="sxs-lookup"><span data-stu-id="b9d4e-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="b9d4e-110">Ročno odprite aplikacijo Intune Company Portal, ki samodejno zažene sinhronizacijo naprave.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="b9d4e-111">Posodobite napravo na Android 6.0 ali višjo različico.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="b9d4e-112">Onemogočite samsung Smart Manager za upravljanje portala Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="b9d4e-113">Preglejte [ta](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) dokument, če želite dodatne podrobnosti o teh težavah in rešitve.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="b9d4e-114">**Vrsta uporabniške licence Neveljavna** ali Uporabniško ime ni **prepoznano:** uporabniku mora biti dodeljena licenca za Intune ali EMS.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b9d4e-115">Preglejte te dokumente, da dodelite licenco prek: Skrbniškega središča za Office ali portala Azure.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="b9d4e-116">Dodatni viri za odpravljanje težave:</span><span class="sxs-lookup"><span data-stu-id="b9d4e-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b9d4e-117">S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b9d4e-118">Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="b9d4e-119">V [tem dokumentu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike.</span><span class="sxs-lookup"><span data-stu-id="b9d4e-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="b9d4e-120">[Preberite, kako včlanite naprave s sistemom Android v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="b9d4e-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
