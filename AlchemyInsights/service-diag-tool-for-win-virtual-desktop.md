---
title: Orodje za diagnostiko storitve za navidezno namizje sistema Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680232"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b99ee-102">Orodje za diagnostiko storitve za navidezno namizje sistema Windows</span><span class="sxs-lookup"><span data-stu-id="b99ee-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b99ee-103">Windows Virtual Desktop (WVD) ponuja diagnostično orodje, ki omogoča, da skrbniki prepoznajo napake z enim samim vmesnikom.</span><span class="sxs-lookup"><span data-stu-id="b99ee-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b99ee-104">To orodje beleži diagnostične informacije, povezane z diagnostiko, kadar WVD uporablja nekdo, ki je dodelil vlogo WVD.</span><span class="sxs-lookup"><span data-stu-id="b99ee-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b99ee-105">Vsak dnevnik vsebuje informacije o vlogi WVD, ki je vključena v dejavnost, sporočila o napakah, ki se pojavijo med sejo, in informacije o najemniku in uporabniku.</span><span class="sxs-lookup"><span data-stu-id="b99ee-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b99ee-106">Analitika v storitvi Azure log je lahko konfigurirana tako, da zajame dnevnik dejavnosti, ki ga je ustvaril diagnostično orodje.</span><span class="sxs-lookup"><span data-stu-id="b99ee-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="b99ee-107">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="b99ee-107">Here's how:</span></span>

1. <span data-ttu-id="b99ee-108">Ustvarjanje delovnega prostora dnevnika Analytics s [portalom Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ali [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="b99ee-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="b99ee-109">[Povežite računalnike s sistemom Windows v storitvi Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="b99ee-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b99ee-110">Pridobite ID delovnega prostora in primarni ključ delovnega prostora.</span><span class="sxs-lookup"><span data-stu-id="b99ee-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b99ee-111">Čarovnik za nastavitev potrebuje te informacije, da pravilno konfigurira posrednika in zagotovi, da lahko komunicira s storitvijo Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="b99ee-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="b99ee-112">[Pritiskajte diagnostične podatke v delovni prostor](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="b99ee-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b99ee-113">Diagnostične podatke iz WVD najemnika lahko potisnete v analizo dnevnika za delovni prostor.</span><span class="sxs-lookup"><span data-stu-id="b99ee-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="b99ee-114">[Prepoznavanje in diagnosticiranje težav](https://go.microsoft.com/fwlink/?linkid=2128338) , ki so notranje ali zunanje glede na WVD.</span><span class="sxs-lookup"><span data-stu-id="b99ee-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b99ee-115">Če želite izvedeti več o konfiguriranju orodja za diagnostiko storitve za WVD, glejte [Uporaba analitike dnevnika za funkcijo diagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="b99ee-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
