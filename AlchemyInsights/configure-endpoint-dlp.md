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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657945"
---
# <a name="configure-endpoint-dlp"></a>Konfiguracija končne točke za DLP

Microsoftova končna točka DLP omogoča razširitev zmogljivosti zaščite in nadzora DLP na občutljive informacije v napravah s sistemom Windows 10. Ko so naprave nameščene v upravljanje naprav, lahko ustvarite pravilnike za zaščito pred zaščito elementov. Raziskovalca dejavnosti je mogoče uporabiti za nadzor dejavnosti za občutljive elemente. Če želite več informacij, glejte [Prenosne naprave v naprave za upravljanje](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Če želite začeti uporabljati DLP končne točke:

- Zagotovite, da imate ustrezno inventarno številko/naročnino za licenciranje. Če želite več informacij, glejte [inventarna številka/licence](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Preverite dovoljenja, ki so zahtevana za upravljanje naprave, dostop do strani za omogočanje ali vklop/izklop nadzora naprave. Če želite več informacij, glejte razdelek [Dodelitev licenc](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- V upravljanje naprav lahko vklopite naprave tako, da upoštevate postopek za prenosne naprave. Če želite več informacij, [informacije o](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Ustvarite pravilnike OLP za zaščito občutljivih elementov. Če želite več informacij, glejte [scenarijev pravilnika o zakasnitve](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Če želite več informacij o preprečevanju izgube podatkov za Microsoft Endpoint DLP, glejte [Več informacij o preprečili izgube podatkov za končne točke storitve Microsoft 365 (predogled)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pomembni koraki za zbiranje podatkov, če je potrebna podpora:**

1. Prenesite [predogled odjemalca MDATP Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Zaženite orodje kot skrbnik v oknu »cmd«:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Ko ste pozvani **z vnesite število minut za zbiranje sledenj:**, vnesite število minut, zahtevanih za zagon scenarija.
1. Zaženite scenarij.

Zberite rezultat datoteke Zip, ki ga daste posredniku za podporo.
