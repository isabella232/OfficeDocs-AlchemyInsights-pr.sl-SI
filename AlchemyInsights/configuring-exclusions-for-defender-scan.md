---
title: Konfiguriranje izjem za Microsoft Defender ATP pregled
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543701"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="ee176-102">Konfiguriranje izjem za Microsoft Defender ATP pregled</span><span class="sxs-lookup"><span data-stu-id="ee176-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="ee176-103">Na splošno lahko nekatere datotečne pripone in mesta map izključite iz Microsoft Defender ATP pregledih.</span><span class="sxs-lookup"><span data-stu-id="ee176-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="ee176-104">Konfigurirate lahko tudi izključitve za datoteke, ki jih je mogoče odpreti z določenimi procesi.</span><span class="sxs-lookup"><span data-stu-id="ee176-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="ee176-105">Če želite več informacij, glejte [Konfiguracija](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) in preverjanje veljavnosti izključitev glede na datotečni pripono in mesto mape in Konfiguracija izključitev za datoteke, [ki jih odprejo postopki.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ee176-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="ee176-106">Če želite konfigurirati izjeme **za Windows Server 2016 in 2019,** [glejte Konfiguracija izključitev Microsoft Defender Antivirus v strežniku Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ee176-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ee176-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="ee176-107">**Mac**</span></span>

<span data-ttu-id="ee176-108">Če želite podrobnosti o podprtih vrstah izključitev in [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) konfiguraciji seznama izjem za računalnike Mac, glejte Podprte vrste izjem in [Konfiguracija seznama izjem.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="ee176-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="ee176-109">**Opomba** S preskusno datoteko EICAR lahko tudi preverite veljavnost seznamov izključitev.</span><span class="sxs-lookup"><span data-stu-id="ee176-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ee176-110">Če želite več informacij, glejte [Preverjanje veljavnosti seznamov izključitev s preskusno datoteko EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="ee176-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="ee176-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="ee176-111">**Linux**</span></span>

<span data-ttu-id="ee176-112">Če želite podrobnosti o podprtih vrstah izključitev in [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) konfiguraciji seznama izjem za Linux, glejte Podprte vrste izjem in Konfiguriraj in preveri veljavnost izjem [za Microsoft Defender ATP za Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="ee176-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="ee176-113">**Opomba** S preskusno datoteko EICAR lahko tudi preverite veljavnost seznamov izključitev.</span><span class="sxs-lookup"><span data-stu-id="ee176-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ee176-114">Če želite več informacij, glejte [Preverjanje veljavnosti seznamov izključitev s preskusno datoteko EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="ee176-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 