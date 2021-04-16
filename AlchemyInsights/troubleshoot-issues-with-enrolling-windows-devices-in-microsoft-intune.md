---
title: Odpravljanje težav z včlanijo naprav s sistemom Windows v storitvi Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808987"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="7d6a6-102">Odpravljanje težav z včlanijo naprav s sistemom Windows v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d6a6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="7d6a6-103">Preglejte vire spodaj, da odpravite težavo.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7d6a6-104">Nekatera pogosta sporočila o napakah in koraki za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="7d6a6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="7d6a6-105">**Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo računa je poteklo.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="7d6a6-106">Znova prenesite paket programske opreme odjemalca za PC v skrbniški konzoli za Intune.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="7d6a6-107">Če želite več informacij, si oglejte to dokumentacijo.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="7d6a6-108">**Koda napake 0x801c0003:** Do napake lahko pride v teh primerih:</span><span class="sxs-lookup"><span data-stu-id="7d6a6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="7d6a6-109">Uporabnik ima včlanitev več naprav, kot je omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7d6a6-110">Preglejte te [dokumente, da odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali spremenite omejitev [naprave.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7d6a6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="7d6a6-111">»Uporabniki lahko naprave pridružijo imeniku Azure AD« je nastavljen na »brez«.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="7d6a6-112">Nastavite jo za vse ali izberite uporabnike.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-112">Set it to all or select users.</span></span> <span data-ttu-id="7d6a6-113">Če [želite več informacij,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) si oglejte to dokumentacijo.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="7d6a6-114">Napravo že včlani drug uporabnik.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="7d6a6-115">V tem primeru odstranite napravo iz konzole Azure Intune ali ročno odstranite napravo, preden poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="7d6a6-116">Naprava je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="7d6a6-117">Imeniku Azure Active Directory se lahko pridružijo le inventavne datoteke (SK) za Windows 10 Pro, Education in Enterprise.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="7d6a6-118">Dodatni viri za odpravljanje težave:</span><span class="sxs-lookup"><span data-stu-id="7d6a6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="7d6a6-119">S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7d6a6-120">Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="7d6a6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="7d6a6-121">V dokumentih si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike: Vodnik za odpravljanje težav [in](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [Odpravljanje težav z dokumentom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="7d6a6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="7d6a6-122">[Preberite, kako včlanite naprave s sistemom Windows v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="7d6a6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
