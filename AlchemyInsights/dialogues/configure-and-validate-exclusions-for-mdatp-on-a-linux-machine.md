---
title: Konfiguriranje in preverjanje izključitve za MDATP v računalniku s sistemom Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696070"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="fd629-102">Konfiguriranje in preverjanje izključitve za MDATP v računalniku s sistemom Linux</span><span class="sxs-lookup"><span data-stu-id="fd629-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="fd629-103">Izključite lahko določene datoteke, mape, procese in procesne datoteke iz MDATP skandiranja.</span><span class="sxs-lookup"><span data-stu-id="fd629-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="fd629-104">Izključitve preprečujejo nepravilne odkrivanje programske opreme in datotek, ki so enolične ali prilagojene za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="fd629-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="fd629-105">Izključitve pripomorejo tudi k ublažitvi težav z učinkovitostjo delovanja, ki jih povzroča MDATP.</span><span class="sxs-lookup"><span data-stu-id="fd629-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="fd629-106">Če želite izvedeti več, glejte [Konfiguriranje in potrjevanje izključitve za MDATP za Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="fd629-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fd629-107">Izključitve, opisane v tem članku, ne veljajo za druge zmogljivosti MDATP za Linux, vključno z zaznavanjem končne točke in odzivom (EDR).</span><span class="sxs-lookup"><span data-stu-id="fd629-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="fd629-108">Datoteke, ki jih izključite z metodami, opisanimi v tem članku, lahko še vedno sprožijo opozorila EDR in druge zmožnosti zaznavanja.</span><span class="sxs-lookup"><span data-stu-id="fd629-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
