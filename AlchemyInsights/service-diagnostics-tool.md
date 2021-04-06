---
title: Orodje za diagnostiko storitve za navidezno namizje sistema Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596047"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="12676-102">Orodje za diagnostiko storitve za navidezno namizje sistema Windows</span><span class="sxs-lookup"><span data-stu-id="12676-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="12676-103">Navidezno namizje sistema Windows (WVD) ponuja diagnostično orodje, ki skrbnikom omogoča, da prepoznajo napake prek enega vmesnika.</span><span class="sxs-lookup"><span data-stu-id="12676-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="12676-104">To orodje beleži diagnostične podatke vsakič, ko nekdo, ki ima dodeljeno vlogo WVD, uporabi WVD.</span><span class="sxs-lookup"><span data-stu-id="12676-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="12676-105">V vsakem dnevniku so informacije o vlogi WVD, ki je vključena v dejavnost, sporočila o napakah, ki se prikažejo med sejo, in informacije o najemniku in uporabniku.</span><span class="sxs-lookup"><span data-stu-id="12676-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="12676-106">Analitiko Azure Log Analytics lahko konfigurirate tako, da zajamete dnevnik dejavnosti, ustvarjen z diagnostičnim orodjem, tako da sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="12676-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="12676-107">Ustvarite delovni prostor Analitike dnevnika s [portalom Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ali [storitvijo Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="12676-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="12676-108">[Povežite računalnike s sistemom Windows z orodjem Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="12676-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="12676-109">Pridobite ID delovnega prostora in primarni ključ delovnega prostora.</span><span class="sxs-lookup"><span data-stu-id="12676-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="12676-110">Čarovnik za nastavitev potrebuje te informacije za pravilno konfiguracijo posrednika in za zagotavljanje, da lahko komunicira z nadzornikom Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="12676-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="12676-111">[Potisnete diagnostične podatke v delovni prostor](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="12676-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="12676-112">Diagnostične podatke lahko potisnete iz najemnika WVD v analitiko dnevnikov za delovni prostor.</span><span class="sxs-lookup"><span data-stu-id="12676-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="12676-113">[Identificirajte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) in diagnosticiraj težave, ki so notranje ali zunanje glede na WVD.</span><span class="sxs-lookup"><span data-stu-id="12676-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="12676-114">Če želite izvedeti več o konfiguraciji orodja za diagnostiko storitve za WVD, glejte Uporaba analitike dnevnikov za diagnostično funkcijo.</span><span class="sxs-lookup"><span data-stu-id="12676-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>