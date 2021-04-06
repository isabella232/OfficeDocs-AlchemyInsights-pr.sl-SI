---
title: Prepoznavanje težav z navideznim namizjem sistema Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596034"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="b5285-102">Prepoznavanje težav z navideznim namizjem sistema Windows</span><span class="sxs-lookup"><span data-stu-id="b5285-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="b5285-103">Navidezna diagnostika namizja sistema Windows uporablja le en ukaz »cmdlet« lupine PowerShell, vendar vsebuje številne izbirne parametre za zoženje in osamite težave.</span><span class="sxs-lookup"><span data-stu-id="b5285-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="b5285-104">Če želite začeti:</span><span class="sxs-lookup"><span data-stu-id="b5285-104">To get started:</span></span> 

1. <span data-ttu-id="b5285-105">Prenesite in uvozite modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b5285-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="b5285-106">Če želite več podrobnosti, glejte [Ukazi »cmdlet« za navidezno namizje sistema Windows za Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="b5285-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="b5285-107">Zaženite ta ukaz »cmdlet« za vpis v svoj račun:</span><span class="sxs-lookup"><span data-stu-id="b5285-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="b5285-108">Primer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="b5285-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="b5285-109">**OPOMBA:** Vse poizvedbe, ki uporabljajo PowerShell, morajo vključevati parametre -UserName ali -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="b5285-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="b5285-110">Za zmogljivosti nadziranja glejte Uporaba [analitike dnevnikov za diagnostično funkcijo](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="b5285-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="b5285-111">Če želite filtrirati diagnostične dejavnosti po uporabniku, zaženite ta ukaz »cmdlet«:</span><span class="sxs-lookup"><span data-stu-id="b5285-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="b5285-112">Primer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="b5285-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="b5285-113">Na voljo je seznam filtrov, s katerih lahko diagnosticirate težave.</span><span class="sxs-lookup"><span data-stu-id="b5285-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="b5285-114">Če želite izvedeti več o diagnosticiranju težav, glejte Prepoznavanje in [diagnosticiranje težav z navideznim namizjem sistema Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="b5285-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="b5285-115">Če želite izvedeti več o pogostih napakah, [glejte Pogoste napake senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="b5285-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
