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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfiguracija nastavitev zasebnosti

Če Microsoft Edge ni nastavljen na platformah, ki niso v sistemu Windows, so na spletnem mestu Microsoft ne pošiljajo diagnostičnih podatkov in informacij o mestu. Če pa je Microsoft Edge uveden v sistemu Windows 10, so podatki o diagnostičnih podatkih in mestu poslani v skladu z [nastavitvami diagnostičnih podatkov uporabnikov sistema Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Če želite konfigurirati, kako Microsoft Edge obravnava zbirko podatkov za vašo organizacijo, uporabite te pravilnike skupine:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ta pravilnik omogoča poročanje o uporabi in nepovezanih podatkih.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ta pravilnik pošlje informacije o mestu, ki se uporabljajo za izboljšanje Microsoftovih storitev.

Če želite izvedeti več, glejte [Konfiguracija nastavitev pravilnika](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).