---
title: Konfiguracija končne točke za DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323934"
---
# <a name="configure-endpoint-dlp"></a>Konfiguracija končne točke za DLP

Microsoftova končna točka DLP omogoča razširitev zmogljivosti zaščite in nadzora DLP na občutljive informacije v napravah s sistemom Windows 10. Ko so naprave nameščene v upravljanje naprav, lahko ustvarite pravilnike za zaščito pred zaščito elementov. Raziskovalca dejavnosti je mogoče uporabiti za nadzor dejavnosti za občutljive elemente. Če želite več informacij, glejte [Prenosne naprave v naprave za upravljanje](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Če želite začeti uporabljati DLP končne točke:

- Zagotovite, da imate ustrezno inventarno številko/naročnino za licenciranje. Če želite več informacij, glejte [inventarna številka/licence](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Preverite dovoljenja, ki so zahtevana za upravljanje naprave, dostop do strani za omogočanje ali vklop/izklop nadzora naprave. Če želite več informacij, glejte razdelek [Dodelitev licenc](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- V upravljanje naprav lahko vklopite naprave tako, da upoštevate postopek za prenosne naprave. Če želite več informacij, [informacije o](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Ustvarite pravilnike OLP za zaščito občutljivih elementov. Če želite več informacij, glejte [scenarijev pravilnika o zakasnitve](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Če želite več informacij o preprečevanju izgube podatkov za Microsoft Endpoint DLP, glejte [Več informacij o preprečili izgube podatkov za končne točke storitve Microsoft 365 (predogled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pomembni koraki za zbiranje podatkov, če je potrebna podpora:**

1. Prenesite [predogled odjemalca MDATP Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Zaženite orodje kot skrbnik v oknu »cmd«:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Ko ste pozvani **z vnesite število minut za zbiranje sledenj:**, vnesite število minut, zahtevanih za zagon scenarija.
1. Zaženite scenarij.

Zberite rezultat datoteke Zip, ki ga daste posredniku za podporo.
