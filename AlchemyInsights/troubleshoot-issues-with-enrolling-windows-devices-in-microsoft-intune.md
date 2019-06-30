---
title: Odpravljanje težav z vpisom naprav Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353553"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0ba93-102">Odpravljanje težav z vpisom naprav Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0ba93-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0ba93-103">Pregledati vire spodaj za zdaj rešiti težavo.</span><span class="sxs-lookup"><span data-stu-id="0ba93-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0ba93-104">Neki splošen zmota vest ter odložnost lestev:</span><span class="sxs-lookup"><span data-stu-id="0ba93-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0ba93-105">**Programske opreme ni mogoče namestiti, 0x80cf4017:** Vaš račun potrdilo je poteklo.</span><span class="sxs-lookup"><span data-stu-id="0ba93-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0ba93-106">Drugi ton oktave-travnato gričevje PC odjemalca programski paket v Admin konzoli Intune.</span><span class="sxs-lookup"><span data-stu-id="0ba93-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0ba93-107">Pregled ta dokumentacija za več informacij.</span><span class="sxs-lookup"><span data-stu-id="0ba93-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="0ba93-108">**Zmota zbornik 0x801c0003:** Napaka se lahko pojavi v naslednjih primerih:</span><span class="sxs-lookup"><span data-stu-id="0ba93-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="0ba93-109">Uporabnik ima več naprav, ki so vpisani presega omejitev naprave.</span><span class="sxs-lookup"><span data-stu-id="0ba93-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0ba93-110">Pregled teh dokumentov [odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0ba93-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="0ba93-111">»Uporabniki lahko pridružijo naprave Azure oglas« nastavljen na "brez".</span><span class="sxs-lookup"><span data-stu-id="0ba93-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="0ba93-112">Jo nastavite na vse ali izberite Uporabniki.</span><span class="sxs-lookup"><span data-stu-id="0ba93-112">Set it to all or select users.</span></span> <span data-ttu-id="0ba93-113">Pregled [ta dokumentacija](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="0ba93-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="0ba93-114">Naprava je vpisan že drug uporabnik.</span><span class="sxs-lookup"><span data-stu-id="0ba93-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0ba93-115">Če je temu tako, odstranite napravo iz Azure Intune konzole ali ročno izpisati napravo, preden poskusite znova.</span><span class="sxs-lookup"><span data-stu-id="0ba93-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="0ba93-116">Naprava je Windows 10 domov.</span><span class="sxs-lookup"><span data-stu-id="0ba93-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0ba93-117">Samo okno 10 Pro, izobraževanje in podjetja SKUs lahko pridruži Azure storitve Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0ba93-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="0ba93-118">Dodatna sredstva za pomoč pri reševanju težave:</span><span class="sxs-lookup"><span data-stu-id="0ba93-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0ba93-119">Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak.</span><span class="sxs-lookup"><span data-stu-id="0ba93-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0ba93-120">Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="0ba93-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="0ba93-121">Pregled teh dokumentov seznam pogostih napak, ki preprečujejo včlanitev in resolucije posameznim: [Priročnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0ba93-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="0ba93-122">[Naučite se, kako vpisati naprav Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="0ba93-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
