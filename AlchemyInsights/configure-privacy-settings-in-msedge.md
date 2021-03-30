---
title: Konfiguracija nastavitev zasebnosti v brskalniku Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405732"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="e8b05-102">Konfiguracija nastavitev zasebnosti v brskalniku Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e8b05-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="e8b05-103">Če je Microsoft Edge uveden v platformah sistema Windows, diagnostični podatki in informacije o mestu privzeto niso poslani Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e8b05-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="e8b05-104">Če pa je Microsoft Edge uveden v sistemu Windows 10, so diagnostični podatki in informacije o mestu poslane v skladu z uporabnikovimi nastavitvami [diagnostičnih podatkov sistema Windows.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="e8b05-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="e8b05-105">Če želite konfigurirati, kako Microsoft Edge obravnava zbiranje podatkov za vašo organizacijo, uporabite te pravilnike skupine:</span><span class="sxs-lookup"><span data-stu-id="e8b05-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="e8b05-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) vklopi poročanje o uporabi in podatkih, povezanih z zrušitvi.</span><span class="sxs-lookup"><span data-stu-id="e8b05-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="e8b05-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) pošlje informacije o mestu, ki se uporabljajo za izboljšanje Microsoftovih storitev.</span><span class="sxs-lookup"><span data-stu-id="e8b05-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="e8b05-108">Če želite več informacij, glejte [Konfiguracija nastavitev pravilnika.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="e8b05-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
