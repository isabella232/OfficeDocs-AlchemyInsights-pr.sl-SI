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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402455"
---
# <a name="configure-endpoint-dlp"></a>Konfiguracija končne točke za DLP

Microsoftova končna točka DLP omogoča razširitev zmogljivosti zaščite in nadzora DLP na občutljive informacije v napravah s sistemom Windows 10. Ko so naprave nameščene v upravljanje naprav, lahko ustvarite pravilnike za zaščito pred zaščito elementov. Raziskovalca dejavnosti je mogoče uporabiti za nadzor dejavnosti za občutljive elemente. Če želite več informacij, glejte [Prenosne naprave v naprave za upravljanje](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Če želite začeti uporabljati DLP končne točke:

- Zagotovite, da imate ustrezno inventarno številko/naročnino za licenciranje. Če želite več informacij, glejte [inventarna številka/licence](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Preverite dovoljenja, ki so zahtevana za upravljanje naprave, dostop do strani za omogočanje ali vklop/izklop nadzora naprave. Če želite več informacij, glejte razdelek [Dodelitev licenc](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- V upravljanje naprav lahko vklopite naprave tako, da upoštevate postopek za prenosne naprave. Če možnost sprejemanja naprav (predogled) v razdelku »Nastavitve skladnosti s predpisi  **storitve M365«**, preverite, ali imate ustrezno licenco in dovoljenja zgoraj. Če želite več informacij, [informacije o](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Ustvarite pravilnike OLP za zaščito občutljivih elementov. Če želite več informacij, glejte [scenarijev pravilnika o zakasnitve](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Če želite več informacij o preprečevanju izgube podatkov za Microsoft Endpoint DLP, glejte [Več informacij o preprečili izgube podatkov za končne točke storitve Microsoft 365 (predogled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pomembni koraki za zbiranje podatkov, če je potrebna podpora:**

1. Prenesite predogled analizatorja za odjemalca MDATP iz storitve [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Zaženite orodje kot skrbnik v oknu »cmd«:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Ko ste pozvani z »Vnesite število minut za zbiranje sledenj: »vnesite število minut, potrebnih za zagon scenarija
5. Zaženite scenarij

Zberite izhod datoteke Zip, ki ga želite dati posredniku za podporo.
