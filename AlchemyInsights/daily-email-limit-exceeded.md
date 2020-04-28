---
title: Presežena je bila dnevna omejitev e-pošte. Potek dela je prekinjen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908720"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevna omejitev e-pošte je presežena. Potek dela je prekinjen.

To napako lahko prejmete v naslednjih scenarijih:

- V programu SharePoint online poteka potek dela, ki uporablja vrsto platforme za potek dela SharePoint 2010 ali SharePoint 2013.
- Potek dela je konfiguriran tako, da pošlje e-poštno sporočilo po meri več kot 200 uporabnikom naenkrat, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.
- Ko zaženete potek dela, e-poštno sporočilo ni poslano in opazite naslednje obnašanje:
    - Za potek dela, ki uporablja vrsto platforme SharePoint 2013, prebrskajte do strani **stanje poteka dela** . Na strani stanje poteka dela je **notranje stanje** nastavljeno na **začeto**in prikaže se oblački z informacijami, ki jih **ni mogoče poslati prejemniku**.

Če želite to težavo narediti, konfigurirajte potek dela za pošiljanje e-poštnih sporočil, ne da bi presegli [omejitve pošiljatelja Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Uporabite na primer premor v poteku dela, pošljite e-poštno sporočilo skupini Microsoft 365, distribucijski skupini ali varnostni skupini, ki je omogočena za pošto, ali pa sporočilo pošljete manj kot 200 prejemnikom naenkrat.


Če želite več informacij, glejte naslednji [članek](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Sorodne teme
- [Ustvari potek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 