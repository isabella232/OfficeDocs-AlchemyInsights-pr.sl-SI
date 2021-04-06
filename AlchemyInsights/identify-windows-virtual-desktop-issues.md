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
# <a name="identify-windows-virtual-desktop-issues"></a>Prepoznavanje težav z navideznim namizjem sistema Windows

Navidezna diagnostika namizja sistema Windows uporablja le en ukaz »cmdlet« lupine PowerShell, vendar vsebuje številne izbirne parametre za zoženje in osamite težave. Če želite začeti: 

1. Prenesite in uvozite modul Windows Virtual Desktop PowerShell. Če želite več podrobnosti, glejte [Ukazi »cmdlet« za navidezno namizje sistema Windows za Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Zaženite ta ukaz »cmdlet« za vpis v svoj račun:
    
    Primer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**OPOMBA:** Vse poizvedbe, ki uporabljajo PowerShell, morajo vključevati parametre -UserName ali -ActivityID. Za zmogljivosti nadziranja glejte Uporaba [analitike dnevnikov za diagnostično funkcijo](https://go.microsoft.com/fwlink/?linkid=2126847).

Če želite filtrirati diagnostične dejavnosti po uporabniku, zaženite ta ukaz »cmdlet«:

Primer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Na voljo je seznam filtrov, s katerih lahko diagnosticirate težave. Če želite izvedeti več o diagnosticiranju težav, glejte Prepoznavanje in [diagnosticiranje težav z navideznim namizjem sistema Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Če želite izvedeti več o pogostih napakah, [glejte Pogoste napake senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
