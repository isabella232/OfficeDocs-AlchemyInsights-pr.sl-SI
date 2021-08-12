---
title: Dnevna omejitev e-pošte je presežena. Potek dela je začasno prekinjen.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914667"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevna omejitev e-pošte je presežena. Potek dela je začasno prekinjen.

To sporočilo o napaki se lahko prikaže v teh primerih:

- V storitvi SharePoint Online je potek dela, ki uporablja vrsto platforme poteka dela SharePoint 2010 ali SharePoint 2013.
- Potek dela je konfiguriran za pošiljanje e-poštnega sporočila po meri več kot 200 uporabnikom hkrati, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.
- Ko zaženete potek dela, e-poštno sporočilo ni poslano, opazili pa boste to delovanje:
    - Za potek dela, ki uporablja vrsto SharePoint 2013, prebrskajte do strani Stanje **poteka** dela. Na strani Stanja poteka dela je notranje **stanje** nastavljeno na Zagnano **,** oblaček z informacijami pa se prikaže Ni mogoče poslati **prejemniku.**

Če želite odpraviti to težavo, konfigurirajte potek dela za pošiljanje e-poštnih sporočil, ne [da bi Exchange Online omejitve pošiljatelja.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Uporabite na primer premor v poteku dela, pošljite e-pošto skupini Microsoft 365, skupini prejemnikov ali varnostni skupini, ki omogoča pošto, ali pošljite sporočilo manj kot 200 prejemnikom hkrati.


Če želite več informacij, glejte ta [članek.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Sorodne teme
- [Ustvarjanje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 