---
title: Omejitev dnevne pošte je presežena. Potek dela je prekinjen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731579"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Omejitev dnevne pošte je presežena. Potek dela je prekinjen.

To napako lahko prejmete v teh primerih:

- V storitvi SharePoint online imate potek dela, ki uporablja vrsto platforme za potek dela za SharePoint 2010 ali SharePoint 2013.
- Potek dela je konfiguriran za pošiljanje e-poštnega sporočila po meri več kot 200 uporabnikom hkrati, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.
- Ko zaženete potek dela, se e-poštno sporočilo ne pošlje in opazite to težavo:
    - Za potek dela z vrsto platforme SharePoint 2013 se pomaknite do strani **stanje poteka dela** . Na strani stanja poteka dela je **stanje notranjega stanja** nastavljeno na **začetek**, oblaček z informacijami pa **ne more poslati prejemniku**.

Če se želite izogniti tej težavi, konfigurirajte potek dela za pošiljanje e-poštnih sporočil, ne da bi presegli [omejitve pošiljatelja Exchange Onlinea](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Uporabite na primer premor v poteku dela, pošljite e-pošto v skupino Microsoft 365, skupino prejemnikov ali varnostno skupino z omogočeno pošto ali pa pošljite sporočilo manj kot 200 prejemnikom hkrati.


Če želite več informacij, si oglejte ta [članek](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Sorodne teme
- [Ustvarjanje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 