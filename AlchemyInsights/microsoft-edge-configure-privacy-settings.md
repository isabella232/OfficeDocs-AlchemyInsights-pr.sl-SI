---
title: Microsoft Edge konfiguracija nastavitev zasebnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678860"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="0394d-102">Microsoft Edge konfiguracija nastavitev zasebnosti</span><span class="sxs-lookup"><span data-stu-id="0394d-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="0394d-103">Če Microsoft Edge ni nastavljen na platformah, ki niso v sistemu Windows, so na spletnem mestu Microsoft ne pošiljajo diagnostičnih podatkov in informacij o mestu.</span><span class="sxs-lookup"><span data-stu-id="0394d-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="0394d-104">Če pa je Microsoft Edge uveden v sistemu Windows 10, so podatki o diagnostičnih podatkih in mestu poslani v skladu z [nastavitvami diagnostičnih podatkov uporabnikov sistema Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="0394d-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="0394d-105">Če želite konfigurirati, kako Microsoft Edge obravnava zbirko podatkov za vašo organizacijo, uporabite te pravilnike skupine:</span><span class="sxs-lookup"><span data-stu-id="0394d-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="0394d-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ta pravilnik omogoča poročanje o uporabi in nepovezanih podatkih.</span><span class="sxs-lookup"><span data-stu-id="0394d-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="0394d-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ta pravilnik pošlje informacije o mestu, ki se uporabljajo za izboljšanje Microsoftovih storitev.</span><span class="sxs-lookup"><span data-stu-id="0394d-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="0394d-108">Če želite izvedeti več, glejte [Konfiguracija nastavitev pravilnika](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="0394d-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>