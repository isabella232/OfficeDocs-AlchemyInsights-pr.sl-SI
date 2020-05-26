---
title: 'AIP skener: namestitev in konfiguracija'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358566"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="e4a7e-102">AIP skener: namestitev in konfiguracija</span><span class="sxs-lookup"><span data-stu-id="e4a7e-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="e4a7e-103">**Za namestitev optičnega bralnika AIP sledite priporočenim smernicam**:</span><span class="sxs-lookup"><span data-stu-id="e4a7e-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="e4a7e-104">Če nadgrajujete in ne izvajate čiste namestitve, preverite, ali ste sledili smernicam za [nadgradnjo aplikacije Azure Information zaščita](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) in za poenoteni odjemalec za označevanje, glejte [Nadgradnja skenerja za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="e4a7e-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="e4a7e-105">Preverite, ali ste skladni z vsemi [zahtevami za nastavitve požarne zidove in omrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="e4a7e-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="e4a7e-106">Prepričajte se, da [so pravilniki nastavljeni](https://docs.microsoft.com/azure/information-protection/configure-policy) na samodejno označevanje ali imajo privzeto oznako v pravilniku.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="e4a7e-107">Prepričajte se, da je ustrezna vrsta datoteke konfigurirana za oznako/zaščito, kot je opisano v [vrstah datotek, ki jih podpira odjemalec Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="e4a7e-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="e4a7e-108">Poleg tega, če želite spremeniti privzeto obnašanje, upoštevajte te smernice: [Spreminjanje privzete ravni zaščite datotek](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="e4a7e-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="e4a7e-109">Preverite, ali ima uporabniški račun, konfiguriran za zagon storitve optičnega bralnika, dovoljenja za dostop do vseh konfiguriranih skladišč.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="e4a7e-110">Če še vedno naletite na težave, prosimo, izvozite dnevnike optičnega bralnika in jih dodajte v vašo podporo vozovnice.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="e4a7e-111">**Izvoz dnevnikov zaščite podatkov Azure**</span><span class="sxs-lookup"><span data-stu-id="e4a7e-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="e4a7e-112">Pluti v%localappdata%\Microsoft\MSIP pod uporabnik zveza tekmovanje v teku radarska antena usluga.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="e4a7e-113">Zip vse vsebine pod MSIP mapo.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="e4a7e-114">Shranite dnevnike na svojo izbiro lokacije in jih priložite zahtevi za storitev.</span><span class="sxs-lookup"><span data-stu-id="e4a7e-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="e4a7e-115">Uporabite lahko tudi [izvozno-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="e4a7e-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="e4a7e-116">**Za dodatne informacije glejte**:</span><span class="sxs-lookup"><span data-stu-id="e4a7e-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="e4a7e-117">Uvajanje skenerja za zaščito podatkov Azure za samodejno razvrščanje in zaščito datotek</span><span class="sxs-lookup"><span data-stu-id="e4a7e-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="e4a7e-118">Določanje in uporaba parametra žetona za» Set-AIPAuthentication «</span><span class="sxs-lookup"><span data-stu-id="e4a7e-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="e4a7e-119">Zaženite cikel odkrivanja in si oglejte poročila za optični bralnik</span><span class="sxs-lookup"><span data-stu-id="e4a7e-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="e4a7e-120">Preglejte dokumentacijo o varstvu podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="e4a7e-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e4a7e-121">Zahteve za zaščito podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="e4a7e-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="e4a7e-122">Prenesite odjemalca za zaščito podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="e4a7e-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
