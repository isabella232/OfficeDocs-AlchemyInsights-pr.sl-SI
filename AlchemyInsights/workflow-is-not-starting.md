---
title: Potek dela se ne začenja
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558001"
---
# <a name="workflow-is-not-starting"></a>Potek dela se ne začenja

- SharePoint 2010 in SharePoint 2013 poteki dela ne začenjajo.

    - Če vaš potek dela ne zažene, lahko pride do začasnih storitev vprašanje če uporabnik pride do občasne zakasnitve z napredkom poteka dela. Preverite [Nadzorna plošča storitev za zdravje](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , da vidim, če vaša organizacija je vplivala.

    - Če več kot 24 ur je minilo, odkar je prvič videl to vprašanje, se prijavite podporo vozovnice. V mnogih primerih, že delamo na rešitev. Prosimo, da nam vsaj 24 ur za dokončanje rešitev.

- Poteki dela za SharePoint 2010 odloži na začetek.

    - To se zgodi, če je potek dela sprožen v velikih serijah. (na primer, ko več so dodani elementi naenkrat).

    - Poteki dela so niso konstruirani za vožnjo v realnem času, tako da zamude pri načrtovanju vedenje.

   -  Če poteka kompleksna Extensible predmet označevalni jezik (XMOL), lahko počasno urejanje. Preverite [ta](https://support.microsoft.com/en-us/kb/3043697) članek.

    - Naj poenostavaiti workflow ali preoblikovanje z tip platforme Microsoft SharePoint 2013 poteka dela.

    - Če zgodovine poteka dela je zrasel velik, morda boste želeli Počisti elemente ali ustvarite nov seznam zgodovine.

        Več informacij: [Počisti zgodovino poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Sorodne teme
Želite poskusiti Microsoft Flow v SharePoint Online?
- [Ustvari tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in pretok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


