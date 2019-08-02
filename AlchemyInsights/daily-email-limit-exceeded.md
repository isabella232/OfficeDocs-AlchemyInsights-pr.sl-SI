---
title: Dnevni email omejitev prekoračena. Potek dela je prekinjena.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059654"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevni email prekoračena. Potek dela je prekinjena.

To napako lahko prejel v naslednjih primerih:

- Imate potek dela v SharePoint Online, ki uporablja SharePoint 2010 ali tip platforme SharePoint 2013 poteka dela.
- Potek dela je nastavljen tako, da po meri email sporočilo poslati več kot 200 uporabnikov naenkrat, več kot 10.000 prejemniki na dan ali več kot 30 sporočil na minuto.
- Ko zaženete potek dela, e-poštno sporočilo ni poslano, in boste opazili naslednje težave:
    - Za potek dela z uporabo tip platforme SharePoint 2013, poiščite stran **Stanja poteka dela** . «Na strani» stanje poteka dela« **Notranje stanje** nastavljeno na **Started**in oblaček z informacijami prikaže **ni mogoče poslati prejemniku**.

Tej težavi, konfigurirajte potek dela za pošiljanje e-poštnih sporočil ne preseže [Exchange Online pošiljatelj omejitve](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primer, uporabite premor v poteku dela, spodbuda email v Office 365 skupine, skupine prejemnikov ali pošte omogočena varnostne skupine ali Pošlji sporočilo manj kot 200 prejemnikom naenkrat.


Če želite več informacij, glejte ta [članek](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Sorodne teme
- [Ustvari tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in pretok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 