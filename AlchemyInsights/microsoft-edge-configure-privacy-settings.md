---
title: Microsoft Edge nastavitev zasebnosti
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114188"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge nastavitev zasebnosti

Če je storitev Microsoft Edge uvedena na platformah, ki ne Windows, Diagnostični podatki in informacije o mestu privzeto niso poslane Microsoftu. Če pa Microsoft Edge v Windows 10, so diagnostični podatki in informacije o mestu poslane glede na uporabnikove [Windows diagnostične podatke.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Če želite konfigurirati Microsoft Edge skrbnik obravnava zbiranje podatkov za vašo organizacijo, uporabite te pravilnike skupine:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)S tem pravilnikom omogočite poročanje o uporabi in podatkih, povezanih z zrušitvi.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ta pravilnik pošilja informacije o mestu, ki se uporabljajo za Microsoftove storitve.

Če želite več informacij, glejte [Konfiguracija nastavitev pravilnika.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)