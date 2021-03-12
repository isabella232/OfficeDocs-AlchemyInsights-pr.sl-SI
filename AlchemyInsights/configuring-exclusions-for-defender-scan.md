---
title: Konfiguriranje izključitve za Microsoft Defender pregled ATP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714352"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="63d44-102">Konfiguriranje izključitve za Microsoft Defender pregled ATP</span><span class="sxs-lookup"><span data-stu-id="63d44-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="63d44-103">Na splošno lahko izključite določene datotečne pripone in mesta map v storitvi Microsoft Defender ATP scans.</span><span class="sxs-lookup"><span data-stu-id="63d44-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="63d44-104">Konfigurirate lahko tudi izključitve za datoteke, ki so bile odprte v določenih procesih.</span><span class="sxs-lookup"><span data-stu-id="63d44-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="63d44-105">Če želite več informacij, si oglejte, [konfigurirajte in preverjajte izključitve, ki temeljijo na datotečni priponi in mestu mape](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) , ter [konfigurirajte izključitve za datoteke, ki so bile odprte s procesi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="63d44-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="63d44-106">Če želite konfigurirati izključitve za  **Windows server 2016 in 2019**, glejte [Konfiguracija izključitve protivirusnega programa Microsoft Defender v sistemu Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="63d44-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="63d44-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="63d44-107">**Mac**</span></span>

<span data-ttu-id="63d44-108">Če želite več informacij o podprtih vrstah izključitve in konfiguriranju seznama izključitve za Mac, glejte [podprte vrste izključitve](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) in [Kako konfigurirate seznam izključitve](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="63d44-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="63d44-109">**Opomba** Izključitvene sezname lahko tudi preverite s preskusno datoteko EICAR.</span><span class="sxs-lookup"><span data-stu-id="63d44-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="63d44-110">Če želite več informacij, si oglejte [preverjanje veljavnosti izključitve seznamov s preskusno datoteko eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="63d44-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="63d44-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="63d44-111">**Linux**</span></span>

<span data-ttu-id="63d44-112">Če želite več informacij o podprtih vrstah izključitve in konfiguriranju seznama izključitve za Linux, glejte [podprte vrste izključitve](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) in [Konfiguracija ter preverjanje izključitve za Microsoft Defender ATP za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="63d44-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="63d44-113">**Opomba** Izključitvene sezname lahko tudi preverite s preskusno datoteko EICAR.</span><span class="sxs-lookup"><span data-stu-id="63d44-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="63d44-114">Če želite več informacij, si oglejte [preverjanje veljavnosti izključitve seznamov s preskusno datoteko eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="63d44-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 